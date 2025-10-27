---
title: Allow Html Lists
second_title: Aspose.Words for JasperReports
articleTitle: Allow Html Lists
linktitle: Allow Html Lists
description: "Aspose Words for JasperReports can convert Html Lists with bullets and numbers."
type: docs
weight: 230
url: /jasperreports/allow-html-lists/
timestamp: 2025-10-27-17-45-04
---

{{% alert color="primary" %}}

By default, value of **ALLOW_HTML_LISTS** parameter is **false**. This means that Aspose Words for JasperReports will replace html bullet and numbering lists with plain text. However, you can enable this option by setting it to **true** if you want convert Html List to Words List. **Note**: this option affects only exporting to DOCX, DOC & RTF output formats.

{{% /alert %}}

**In JasperReports:**

{{< highlight java >}}
import com.aspose.words.jasperreports.*;
AWDocExporter exporter = new AWDocExporter();
exporter.setParameter(AWExporterParameter.ALLOW_HTML_LISTS, true);
exporter.exportReport();
{{< /highlight >}}

**In JasperServer:**

{{< highlight html >}}
<bean id="aw_exportParameters" class="com.aspose.words.jasperreports.AWExportParametersBean">
    <property name="allowHtmlLists" value="true"/>
</bean>
{{< /highlight >}}
