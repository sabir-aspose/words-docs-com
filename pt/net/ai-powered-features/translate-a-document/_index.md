---
title: Traduzir um documento
second_title: Aspose.Words para .NET
articleTitle: Traduzir um documento
linktitle: Traduzir um documento
type: docs
weight: 30
description: "Traduzir um documento. Aspose.Words for .NET simplifica a tradução de documentos utilizando os modelos de IA do Google, permitindo especificar o idioma de destino."
url: /pt/net/traduzir-um-documento/
timestamp: 2024-12-13-06-40-00
---

A tradução de documentos é uma opção frequentemente necessária na era da alta digitalização. O Aspose.Words suporta a tradução de documentos utilizando modelos de linguagem generativos do *Google*, que permitem aos programadores traduzir conteúdo de textos em mais de 300 idiomas.

Utilize o método [Traduzir](https://reference.aspose.com/words/net/aspose.words.ai/iaimodeltext/translate/) para traduzir os seus documentos para qualquer idioma representado no [Língua](https:// reference .aspose.com/words/net/aspose.words.ai/language/) enumeração. Note que se o documento de origem contiver vários idiomas, o modelo baseado em IA da Google será capaz de traduzir todos os idiomas suportados. Se o modelo não conseguir reconhecer o idioma em alguns fragmentos de texto, receberá um documento com esses fragmentos não traduzidos e com o restante texto traduzido.

O exemplo de código seguinte mostra como utilizar o modelo *Gemini 1.5 Flash* em Aspose.Words para traduzir um documento para árabe:

{{< highlight csharp >}}
Document doc = new Document(MyDir + "Document.docx");

string apiKey = Environment.GetEnvironmentVariable("API_KEY");
// Use Google generative language models.
IAiModelText model = (IAiModelText)AiModel.Create(AiModelType.Gemini15Flash).WithApiKey(apiKey);

Document translatedDoc = model.Translate(doc, Language.Arabic);
translatedDoc.Save(ArtifactsDir + "AI.AiTranslate.docx");
{{< /highlight >}}

{{% alert color="primary" %}}

A tradução de documentos com o Aspose.Words poupa tempo e facilita a integração da funcionalidade de tradução nos seus projetos. Para mais informações, consulte a documentação da API [Aspose.Words.AI](https://reference.aspose.com/words/net/aspose.words.ai/).

{{% /alert %}}