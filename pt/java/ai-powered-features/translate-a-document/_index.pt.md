---
title: Traduzir um documento
second_title: Aspose.Words Para Java
articleTitle: Traduzir um documento
linktitle: Traduzir um documento
type: docs
weight: 30
description: "Traduzir um documento. Aspose.Words Para Java simplifica a tradução de documentos utilizando os modelos Google AI, permitindo especificar o idioma de destino."
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /pt/java/translate-a-document/
timestamp: 2025-03-17-19-00-00
---

A tradução de documentos é uma opção frequentemente necessária na era da alta digitalização. Aspose.Words oferece suporte à tradução de documentos usando *Google* modelos de linguagem generativa, o que permite aos desenvolvedores traduzir o conteúdo de textos para mais de 300 idiomas.

Utilize o método [Translate](https://reference.aspose.com/words/java/com.aspose.words/iaimodeltext/#translate-com.aspose.words.Document-int) para traduzir os seus documentos para qualquer língua representada na enumeração [Language](https://reference.aspose.com/words/java/com.aspose.words/language/). Observe que, se o documento de origem contiver vários idiomas, o modelo baseado no Google AI poderá traduzir todos os idiomas suportados. Se o modelo não puder reconhecer o idioma em alguns fragmentos de texto, ser-lhe-á devolvido um documento com esses fragmentos não traduzidos e com o resto do texto traduzido.

O exemplo de código a seguir mostra como usar o modelo *Gemini 1.5 Flash* em Aspose.Words para traduzir um documento para o árabe:

{{< highlight java >}}
Document doc = new Document("Document.docx");

String apiKey = System.getenv("API_KEY");
 IAiModelText model = (IAiModelText)AiModel.create(AiModelType.GEMINI_15_FLASH).withApiKey(apiKey);

Document translatedDoc = model.translate(doc, Language.ARABIC);
translatedDoc.save("AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

Traduzir documentos com Aspose.Words poupa tempo e facilita a integração da funcionalidade de Tradução nos seus projetos. Para mais informações, verifique o [Java API documentation](https://reference.aspose.com/words/java/com.aspose.words/).

{{% /alert %}}