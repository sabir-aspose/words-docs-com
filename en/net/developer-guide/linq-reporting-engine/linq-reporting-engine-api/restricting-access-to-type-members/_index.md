---
title: Restricting Access to Type Members in C#
second_title: Aspose.Words for .NET
articleTitle: Restricting Access to Type Members
linktitle: Restricting Access to Type Members
description: "Learn how to restrict access of a template author to members of types sensitive using LINQ in C#."
type: docs
weight: 90
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /net/restricting-access-to-type-members/
timestamp: 2024-01-27-14-07-04
---

{{% alert color="grey" %}}

*Purpose Summary. What is this page about?*

This page explains how to restrict access to external type members when using the Reporting Engine.

{{% /alert %}}

In scenarios where report templates are created by a third party, it can make sense to restrict access of a template author to members of types sensitive from a security point of view. LINQ Reporting Engine provides API to accomplish this as illustrated with the following example. Given that `SomeClass1` and `SomeClass2` are types which members should be inaccessible by the engine through template syntax, you can use the following code snippet to make the engine restrict the access.

{{< highlight csharp >}}
ReportingEngine.SetRestrictedTypes(typeof(SomeClass1), typeof(SomeClass2));
{{< /highlight >}}

After the code is run, on attempt to access any member of types `SomeClass1` and `SomeClass2` through a template, there are two possible outcomes while building a report:

1. By default, the engine throws an exception saying about a syntactic error the same way it does when encounters a missing type member.
1. If missing type members are allowed, the engine treats every such a member as a null literal (see “Accessing Missing Members of Data Objects” for more information).

**Note** – The engine also restricts access to members of types derived from `SomeClass1` and `SomeClass2` in the same way.

Restricted types can be set only before building the very first report. Once restricted types are checked for the first time while building a report, they cannot be changed after that and an exception is thrown on attempt to do this. That is why, the recommended place to set restricted types is your application’s startup.

**Note** – To determine whether access to a particular type member should be restricted, some reflective calls are done by the engine under the hood, so for better performance, it is recommended to keep the set of restricted types minimal by restricting access to members of only those types that are crucial in terms of security.

------ 

## FAQ

1. **Q:** How do I restrict access to specific type members in the Reporting Engine?  
   **A:** Call `ReportingEngine.SetRestrictedTypes` and pass the `Type` objects of the classes whose members must be hidden. This method must be invoked before any report is built.

2. **Q:** When is the appropriate time to call `SetRestrictedTypes`?  
   **A:** It should be executed during application startup, before the first report generation, because the restriction list is locked after the engine processes the first template.

3. **Q:** What happens if a template tries to use a restricted member?  
   **A:** By default the engine throws a syntax‑error exception, indicating that the member is unavailable. If the engine is configured to allow missing members, the restricted member is treated as `null` instead of throwing.

4. **Q:** Can I modify the list of restricted types after a report has been built?  
   **A:** No. Once the engine has validated the restricted types during the first report build, any subsequent attempt to change the list results in an exception.

5. **Q:** Does the restriction also apply to classes derived from a restricted type?  
   **A:** Yes. All members of derived classes are automatically treated as restricted, providing consistent protection across the inheritance hierarchy.