---
title: Résumer un document
second_title: Aspose.Words pour Python via .NET
articleTitle: Résumer un document
linktitle: Résumer un document
type: docs
weight: 20
description: "Résumez un document. Aspose.Words pour Python simplifie la synthèse des documents à l'aide des modèles OpenAI et Google AI en vous permettant de spécifier la longueur du résumé."
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /fr/python-net/summarize-a-document/
timestamp: 2025-03-17-19-00-00
---

La synthèse des documents est un outil précieux pour l'examen du contenu, des informations rapides ou la préparation des résumés. Aspose.Words prend en charge la synthèse des documents à l'aide de modèles alimentés par AI, ce qui facilite le traitement du texte long. Cette fonctionnalité, disponible dans le module [aspose.words.ai](https://reference.aspose.com/words/python-net/aspose.words.ai/), intègre des modèles de langage génératif avancés de *OpenAI* et *Google*, ainsi que des modèles de langage génératif anthropique *Claude's*. La liste des modèles pris en charge est disponible dans l'énumération [AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/).

Vous pouvez spécifier diverses options pour résumer le contenu du document. Utilisez la méthode [summarize](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/summarize/) pour générer un résumé de votre document. Vous pouvez également définir la longueur du résumé à l'aide de la propriété [summary_length](https://reference.aspose.com/words/python-net/aspose.words.ai/summarizeoptions/summary_length/).

Avec Aspose.Words, la mise en œuvre de la synthèse des documents est simple. L'exemple de code suivant montre comment résumer un document à l'aide du modèle GPT-4o:

{{< highlight python >}}
first_doc = aw.Document(MyDir + "Big document.docx")
second_doc = aw.Document(MyDir + "Document.docx")
api_key = os.getenv("API_KEY")
# Use OpenAI or Google generative language models.
model = aw.ai.AiModel.create(aw.ai.AiModelType.GPT_4O_MINI).with_api_key(api_key).as_open_ai_model()
options = aw.ai.SummarizeOptions()
options.summary_length = aw.ai.SummaryLength.SHORT
one_document_summary = model.summarize(first_doc, options)
oneDocumentSummary.save(ArtifactsDir + "AI.AiSummarize.One.docx")
options.summary_length = aw.ai.SummaryLength.LONG
multi_document_summary = model.summarize([first_doc, second_doc], options)
multiDocumentSummary.save(ArtifactsDir + "AI.AiSummarize.Multi.docx")
{{< /highlight >}}

{{% alert color="primary" %}}

Résumer des documents avec Aspose.Words vous fait gagner du temps et vous aide à vous concentrer sur les informations essentielles. Pour plus d'informations, consultez la documentation [aspose.words.ai](https://reference.aspose.com/words/python-net/aspose.words.ai/) API.

{{% /alert %}}