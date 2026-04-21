---
title: Restarting List Numbering Dynamically in C#
second_title: Aspose.Words for .NET
articleTitle: Restarting List Numbering Dynamically
linktitle: Restarting List Numbering Dynamically
description: "Restart list numbering within your documents dynamically when building a report using C#."
type: docs
weight: 110
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/restarting-list-numbering-dynamically/
aliases: [/net/template-syntax/#restarting-list-numbering-dynamically]
timestamp: 2024-02-16-10-54-23
---

{{% alert color="grey" %}}

## Purpose Summary

This page explains how to restart list numbering dynamically during templated document generation.

{{% /alert %}}

You can restart list numbering within your documents dynamically using `restartNum` tags. In particular, this feature is useful when working with a nested numbered list within a data band as shown in the following example.

Assume that you have the `Order` and `Service` classes defined in your application as follows.

{{< highlight csharp >}}
  public class Order
  {
    public String ClientName { get { ... } }
    public String ClientAddress { get { ... } }
    public IEnumerable<Service> Services { get { ... } }
    ...
  }

  public class Service
  {
    public String Name { get { ... } }
    ...
  }
{{< /highlight >}}

Given that `orders` is an enumeration of `Order` instances, you could try to use the following template to output information on several orders in one document.

{{< highlight csharp >}}
<<foreach [order in orders]>><<[order.ClientName]>> (<<[order.ClientAddress]>>)

1. <<foreach [service in order.Services]>><<[service.Name]>>

<</foreach>><</foreach>>
{{< /highlight >}}

But then, a result document would look as follows.

{{< highlight text >}}
Jane Doe (445 Mount Eden Road Mount Eden Auckland 1024)

1. Regular Cleaning
2. Oven Cleaning

John Smith (43 Vogel Street Roslyn Palmerston North 4414)

3. Regular Cleaning

4. Oven Cleaning

5. Carpet Cleaning
   {{< /highlight >}}

That is, there would be a single numbered list across all orders, which is not applicable for this scenario. However, you can make list numbering to restart for every order by putting a `restartNum` tag into your template before a corresponding `foreach` tag as follows.

{{< highlight csharp >}}
<<foreach [order in orders]>><<[order.ClientName]>> (<<[order.ClientAddress]>>)

	1. <<restartNum>><<foreach [service in order.Services]>><<[service.Name]>>

<</foreach>><</foreach>>
{{< /highlight >}}

**Note** – When using with a data band, it is required to put a `restartNum` tag before a corresponding a `foreach` tag in the same numbered paragraph.

Then, a result document looks as follows.
{{< highlight text >}}
Jane Doe (445 Mount Eden Road Mount Eden Auckland 1024)**

1. Regular Cleaning
2. Oven Cleaning

John Smith (43 Vogel Street Roslyn Palmerston North 4414)

3. Regular Cleaning
4. Oven Cleaning
5. Carpet Cleaning
{{< /highlight >}}

**Note** – You can use a `restartNum` tag without a data band to dynamically restart list numbering for a containing paragraph, if needed; for example, the tag can be used to restart list numbering for a document inserted dynamically (see “Inserting Documents Dynamically” for more information).

------ 

## FAQ

1. **Q:** How do I restart list numbering for each iteration of a `foreach` loop?  
   **A:** Place the `<<restartNum>>` tag immediately before the `<<foreach>>` tag that generates the list items. The tag must be inside the same numbered paragraph, so the numbering restarts when the loop begins for each new parent element.

2. **Q:** Can the `restartNum` tag be used when there is no data band (no `foreach`)?  
   **A:** Yes. `<<restartNum>>` can be inserted in any numbered paragraph to reset the list numbering at that point, even if the paragraph is not part of a data band. This is useful for inserting externally generated content that should start a new list.

3. **Q:** What happens if I put `<<restartNum>>` inside a nested list?  
   **A:** The tag restarts numbering for the list that contains the paragraph where it appears. If placed inside a nested list, only that nested list’s numbering is reset, while outer list numbering continues unaffected. Ensure the tag is positioned in the correct paragraph to achieve the desired reset scope.