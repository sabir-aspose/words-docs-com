---
title: Traduzir um documento
second_title: Aspose.Words para Python via .NET
articleTitle: Traduzir um documento
linktitle: Traduzir um documento
type: docs
weight: 30
description: "Traduzir um documento. Aspose.Words Para Python simplifica a tradução de documentos utilizando os modelos Google AI, permitindo especificar o idioma de destino."
url: /pt/python-net/translate-a-document/
timestamp: 2025-01-15-16-40-05
---

A tradução de documentos é uma opção frequentemente necessária na era da alta digitalização. Aspose.Words oferece suporte à tradução de documentos usando *Google* modelos de linguagem generativa, o que permite aos desenvolvedores traduzir o conteúdo de textos para mais de 300 idiomas.

Utilize o método [Translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/#document_language) para traduzir os seus documentos para qualquer língua representada na enumeração [Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/). Observe que, se o documento de origem contiver vários idiomas, o modelo baseado no Google AI poderá traduzir todos os idiomas suportados. Se o modelo não puder reconhecer o idioma em alguns fragmentos de texto, ser-lhe-á devolvido um documento com esses fragmentos não traduzidos e com o resto do texto traduzido.

O exemplo de código a seguir mostra como usar o modelo *Gemini 1.5 Flash* em Aspose.Words para traduzir um documento para o árabe:

{{< highlight csharp >}}
doc = aw.Document(file_name=MY_DIR + "Document.docx")

api_key = system_helper.environment.Environment.get_environment_variable("API_KEY")
# Use Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GEMINI_15_FLASH).with_api_key(api_key).as_google_ai_model()

translated_doc = model.translate(doc, aw.ai.Language.ARABIC)
translated_doc.save(file_name=ARTIFACTS_DIR + "AI.AiTranslate.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Traduzir documentos com Aspose.Words poupa tempo e facilita a integração da funcionalidade de Tradução nos seus projetos. Para obter mais informações, consulte a documentação [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}