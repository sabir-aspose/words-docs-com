---
title: Превод на документ
second_title: Aspose.Words за Python via .NET
articleTitle: Превод на документ
linktitle: Превод на документ
type: docs
weight: 30
description: "Превод на документ. Aspose.Words за Python опростява превода на документи с помощта на Гугъл AI модели, което ви позволява да определите целевия език."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /bg/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

Преводът на документи е често необходима опция в ерата на висока дигитализация. Aspose.Words поддържа превод на документи, използвайки *Google* генеративни езикови модели, което позволява на разработчиците да превеждат текстово съдържание на повече от 300 езика.

Използвайте метода [Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language), за да преведете документите си на всеки език, представен в списъка [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/). Обърнете внимание, че ако изходният документ съдържа няколко езика, моделът на Гугъл AI ще може да превежда всички поддържани езици. Ако моделът не може да разпознае езика в някои текстови фрагменти, тогава ще ви бъде върнат документ с тези непреведени фрагменти и с останалата част от текста, преведена.

Следващият пример за код показва как да използвате модела *Gemini 1.5 Flash* във Aspose.Words, За да преведете документ на арабски:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Преводът на документи с Aspose.Words спестява време и улеснява интегрирането на функционалност за превод във вашите проекти. За повече информация вижте документацията [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}