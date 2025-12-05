---
title: Low Code
second_title: Aspose.Wordsper .NET
articleTitle: Lavorare con i documenti usando LowCode API
linktitle: Low Code
type: docs
description: "Semplifica le attività di elaborazione dei documenti come confronta, converti, dividi, unisci, trova e sostituisci e altre utilizzando Low Code API. Aspose.Words LowCode API con sintassi pulita, risultati rapidi e sforzo di codifica minimo."
weight: 33
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /it/net/low-code/
timestamp: 2025-04-22-07-08-55
---

Aspose.Wordsper .NET fornisce lo spazio dei nomi [Aspose.Words.LowCode](https://reference.aspose.com/words/net/aspose.words.lowcode/), che semplifica le attività comuni di elaborazione dei documenti. Questo API è progettato per gli sviluppatori che desiderano eseguire operazioni di alto livello come il confronto dei documenti, l'estrazione del contenuto, la conversione delle immagini e la sostituzione del testo con il minimo sforzo.

LowCode API è ideale per scenari in cui l'implementazione rapida è più importante del controllo a grana fine. Diamo un'occhiata più da vicino alle capacità LowCode di Aspose.Wordsper .NET.

{{% alert color="primary" %}}

È importante notare che LowCode API non consente di modificare la struttura del documento.

{{% /alert %}}

## Funzioni disponibili in LowCode API

Lo spazio dei nomi `Aspose.Words.LowCode` attualmente supporta:

* **Converting** documenti da un formato all'altro
* **Comparing** documenti
* **Mail merging**
* **Reporting** basato sulla sintassi LINQ
* **Merging** documenti
* **Search and replace**
* **Digital signing** di documenti
* **Splitting** un documento in parti utilizzando criteri diversi
* Aggiunta di un **watermark**

{{% alert color="primary" %}}

Si prega di notare che una descrizione dettagliata di ogni funzione al di fuori di Low Code può essere trovata nella sezione Guida per gli sviluppatori.

{{% /alert %}}

## Fluente e non fluente API

Aspose.Wordsper .NET supporta sia Fluente che non fluente APIs, consentendo agli sviluppatori di scegliere lo stile che meglio si adatta alle loro preferenze di codifica e alle esigenze del progetto. Diamo un'occhiata ad alcuni esempi per vedere come questi due tipi di API differiscono.

{{% alert color="primary" %}}

In Fluent API, le operazioni possono essere configurate ed eseguite attraverso un contesto (ad esempio ComparerContext o ReplacerContext). Questo contesto contiene opzioni comuni. Garantisce che tutti i metodi correlati operino con una configurazione coerente, rendendo API potente e facile da gestire in scenari complessi.

{{% /alert %}}

### Confronta documenti

Utilizzare `LowCode` per confrontare due documenti Word e salvare il risultato.

**esempio di api non fluente:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc);
{{< /highlight >}}

**esempio di api fluente:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

Comparer.Create()
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.1.docx")
   .Execute();
{{< /highlight >}}

Puoi anche passare `CompareOptions` per un confronto ottimizzato.

**esempio di api non fluente:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

CompareOptions options = new CompareOptions
{
    IgnoreFormatting = true,
    IgnoreCaseChanges = true
};

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc, options);
{{< /highlight >}}

**esempio di api fluente:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

ComparerContext comparerContext = new ComparerContext();
comparerContext.CompareOptions.IgnoreCaseChanges = true;

Comparer.Create(comparerContext)
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.3.docx")
   .Execute();
{{< /highlight >}}

### Converti documenti in immagini

Usare `LowCode` per convertire Word documento in PDF.

**esempio di api non fluente:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Convert(inputDoc, outputDoc);
{{< /highlight >}}

**esempio di api fluente:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Create()
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

### Trovare e sostituire il testo

Utilizzare `LowCode` per sostituire rapidamente il testo nell'intero documento.

**esempio di api non fluente:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";
string pattern = "Aspose";
string replacement = "Aspose Pro";

Replacer.Replace(inputDoc, outputDoc, pattern, replacement);
{{< /highlight >}}

**esempio di api fluente:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";

ReplacerContext replacerContext = new ReplacerContext();
replacerContext.SetReplacement("ReplaceMe", "Replacement");

Replacer.Create(replacerContext)
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

## Perché usare Aspose.Words Low Code

Lo spazio dei nomi **Aspose.Words.LowCode** consente di implementare rapidamente attività di elaborazione di documenti di alto livello con una sintassi pulita e leggibile. È particolarmente utile per gli sviluppatori che hanno bisogno di velocità, semplicità e codice mantenibile quando lavorano con documenti Word.

Per esplorare opzioni più avanzate, è sempre possibile combinare LowCode APIs con il modello a oggetti completo Aspose.Words. Vedi altri esempi Low Code nel [API documentation](https://reference.aspose.com/words/net/aspose.words.lowcode/).