---
title: خلاصه یک سند
second_title: Aspose.Words برای C++
articleTitle: خلاصه یک سند
linktitle: خلاصه یک سند
type: docs
weight: 20
description: "یک سند را خلاصه کنید. Aspose.Words برای C++ خلاصه سازی اسناد را با استفاده از مدل های OpenAI و Google AI ساده می کند و به شما اجازه می دهد طول خلاصه را مشخص کنید."
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fa/cpp/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

خلاصه کردن اسناد ابزاری ارزشمند برای بررسی محتوا، بینش سریع یا تهیه خلاصه است. Aspose.Words از خلاصه سازی اسناد با استفاده از مدل های AI پشتیبانی می کند و پردازش متن طولانی را آسان تر می کند. این ویژگی که در فضای نام [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) موجود است، مدل های پیشرفته زبان تولید را از *OpenAI* و *Google* و همچنین مدل های زبان تولید انسان *Claude's* ادغام می کند. لیست مدل های پشتیبانی شده در فهرست [AiModelType](https://reference.aspose.com/words/cpp/aspose.words.ai/aimodeltype/) موجود است.

شما می توانید گزینه های مختلفی را برای خلاصه کردن محتوای سند مشخص کنید. از روش [Summarize](https://reference.aspose.com/words/cpp/aspose.words.ai/iaimodeltext/summarize/) برای ایجاد خلاصه ای از سند خود استفاده کنید. همچنین می توانید طول خلاصه را با استفاده از ویژگی [SummaryLength](https://reference.aspose.com/words/cpp/aspose.words.ai/summarizeoptions/get_summarylength/) تنظیم کنید.

با Aspose.Words، خلاصه سازی اسناد پیاده سازی ساده است. مثال کد زیر نشان می دهد که چگونه یک سند را با استفاده از مدل GPT-4o خلاصه کنیم:

{{< highlight cpp >}}
void AiSummarize()
{
    auto firstDoc = MakeObject<Document>(MyDir + u"Big document.docx");
    auto secondDoc = MakeObject<Document>(MyDir + u"Document.docx");

    SharedPtr<IAiModelText> model = System::ExplicitCast<OpenAiModel>(MakeObject<AiModel>()->Create(AiModelType::Gpt4OMini)->WithApiKey(u"API_KEY"))->WithOrganization(u"Organization")->WithProject(u"Project");

    auto options = MakeObject<SummarizeOptions>();

    options->set_SummaryLength(SummaryLength::Short);
    auto firstDocumentSummary = model->Summarize(firstDoc, options);
    firstDocumentSummary->Save(ArtifactsDir + u"AI.AiSummarize.One.docx");

    System::ArrayPtr<System::SharedPtr<Document>> documents = System::MakeArray<System::SharedPtr<Document>>(2);
    documents[0] = firstDoc;
    documents[1] = secondDoc;

    options->set_SummaryLength(SummaryLength::Long);
    auto multiDocumentSummary = model->Summarize(documents, options);
    firstDocumentSummary->Save(ArtifactsDir + u"AI.AiSummarize.Multi.docx");
}
{{< /highlight >}}

{{% alert color="primary" %}}

خلاصه کردن اسناد با Aspose.Words زمان را صرفه جویی می کند و به شما کمک می کند تا بر روی اطلاعات ضروری تمرکز کنید. برای اطلاعات بیشتر، اسناد [Aspose.Words.AI](https://reference.aspose.com/words/cpp/aspose.words.ai/) API را بررسی کنید.

{{% /alert %}}
