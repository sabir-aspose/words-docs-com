---
title: Превод на документ
second_title: Aspose.Words за Java
articleTitle: Превод на документ
linktitle: Превод на документ
type: docs
weight: 30
description: "Превод на документ. Aspose.Words за Java опростява превода на документи с помощта на Гугъл AI модели, което ви позволява да определите целевия език."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /bg/java/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

Преводът на документи е често необходима опция в ерата на висока дигитализация. Aspose.Words поддържа превод на документи, използвайки *Google* генеративни езикови модели, което позволява на разработчиците да превеждат текстово съдържание на повече от 300 езика.

Използвайте метода [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int), за да преведете документите си на всеки език, представен в списъка [Language](https://reference.aspose.com/words/java/com.aspose.words/language/). Обърнете внимание, че ако изходният документ съдържа няколко езика, моделът на Гугъл AI ще може да превежда всички поддържани езици. Ако моделът не може да разпознае езика в някои текстови фрагменти, тогава ще ви бъде върнат документ с тези непреведени фрагменти и с останалата част от текста, преведена.

Следващият пример за код показва как да използвате модела *Gemini 1.5 Flash* във Aspose.Words, За да преведете документ на арабски:

{{< highlight java >}}
Document doc = new Document("Document.docx");

String apiKey = System.getenv("API_KEY");
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GEMINI_15_FLASH).withApiKey(apiKey);

Document translatedDoc = model.translate(doc, Language.ARABIC);
translatedDoc.save("AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Преводът на документи с Aspose.Words спестява време и улеснява интегрирането на функционалност за превод във вашите проекти. За повече информация вижте [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}