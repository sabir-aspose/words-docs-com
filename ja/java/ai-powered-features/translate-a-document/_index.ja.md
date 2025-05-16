---
title: 文書を翻訳する
second_title: Aspose.WordsのためのJava
articleTitle: 文書を翻訳する
linktitle: 文書を翻訳する
type: docs
weight: 30
description: "文書を翻訳します。 Aspose.WordsのためのJava GoogleAIモデルを使用して文書翻訳を簡素化し、ターゲット言語を指定できるようにします。"
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /ja/java/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

文書翻訳は、高度なデジタル化の時代に頻繁に必要とされるオプションです。 Aspose.Wordsは、*Google*生成言語モデルを使用した文書翻訳をサポートし、開発者はテキストコンテンツを300以上の言語に翻訳することができます。

ドキュメントを[Language](https://reference.aspose.com/words/java/com.aspose.words/language/)列挙体で表される任意の言語に変換するには、[Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int)メソッドを使用します。 ソース文書に複数の言語が含まれている場合、GoogleAIベースのモデルはサポートされているすべての言語を翻訳できることに注意してください。 モデルが一部のテキストフラグメントで言語を認識できない場合は、これらの翻訳されていないフラグメントと残りのテキストが翻訳された文書が返されます。

次のコード例は、Aspose.Wordsの*Gemini 1.5 Flash*モデルを使用して文書をアラビア語に翻訳する方法を示しています:

{{< highlight java >}}
Document doc = new Document("Document.docx");

String apiKey = System.getenv("API_KEY");
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GEMINI_15_FLASH).withApiKey(apiKey);

Document translatedDoc = model.translate(doc, Language.ARABIC);
translatedDoc.save("AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Aspose.Wordsを使用して文書を翻訳すると、時間が節約され、翻訳機能をプロジェクトに簡単に統合できます。 詳細については、[Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/)を確認してください。

{{% /alert %}}