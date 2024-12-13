---
title: Превод на документ
second_title: Aspose.Words за .NET
articleTitle: Превод на документ
linktitle: Превод на документ
type: docs
weight: 30
description: "Преведете документ. Aspose.Words за .NET опростява превода на документи с помощта на модели на Google AI, което ви позволява да посочите целевия език."
url: /bg/net/translate-a-document/
timestamp: 2024-12-13-06-40-00
---

Преводът на документи е често необходима опция в ерата на високата дигитализация. Aspose.Words поддържа превод на документи с помощта на *Google* генеративни езикови модели, което позволява на разработчиците да превеждат текстово съдържание на повече от 300 езика.

Използвайте метода [Translate](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/), за да преведете вашите документи на всеки език, представен на [Language](https:// reference.aspose.com/words/net/aspose.words.ai/language/) изброяване. Обърнете внимание, че ако изходният документ съдържа няколко езика, базираният на Google AI модел ще може да превежда всички поддържани езици. Ако моделът не може да разпознае езика в някои текстови фрагменти, тогава ще ви бъде върнат документ с тези непреведени фрагменти и с преведен останалата част от текста.

Следният пример на код показва как да използвате модела *Gemini 1.5 Flash* в Aspose.Words за превод на документ на арабски:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Преводът на документи с Aspose.Words спестява време и улеснява интегрирането на функционалността за превод във вашите проекти. За повече информация проверете [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/) документацията за API.

{{% /alert %}}