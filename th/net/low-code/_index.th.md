---
title: Low Code
second_title: Aspose.Wordsสำหรับ.NET
articleTitle: ทำงานกับเอกสารโดยใช้LowCodeAPI
linktitle: Low Code
type: docs
description: "ลดความซับซ้อนของงานการประมวลผลเอกสารเช่นเปรียบเทียบ,แปลง,แยก,ผสาน,ค้นหาและแทนที่,และอื่นๆโดยใช้Low CodeAPI. Aspose.WordsLowCodeAPIด้วยไวยากรณ์ที่สะอาด,ผลลัพธ์ที่รวดเร็ว,และความพยายามในการเขียนโค้ดน้อยที่สุด."
weight: 33
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /th/net/low-code/
timestamp: 2025-04-22-07-08-55
---

Aspose.Wordsสำหรับ.NET จัดเตรียมเนมสเปซ[Aspose.Words.LowCode](https://reference.aspose.com/words/net/aspose.words.lowcode/)ซึ่งทำให้งานประมวลผลเอกสารทั่วไปง่ายขึ้น APIนี้ถูกออกแบบมาสำหรับนักพัฒนาที่ต้องการดำเนินการในระดับสูงเช่นการเปรียบเทียบเอกสาร,การสกัดเนื้อหา,การแปลงภาพ,และการเปลี่ยนข้อความด้วยความพยายามน้อยที่สุด.

LowCodeAPIเหมาะสำหรับสถานการณ์ที่การดำเนินการอย่างรวดเร็วมีความสำคัญมากกว่าการควบคุ ลองมาดูที่LowCodeความสามารถของ Aspose.Wordsสำหรับ.NET.

{{% alert color="primary" %}}

สิ่งสำคัญคือต้องทราบว่าLowCodeAPIไม่อนุญาตให้คุณเปลี่ยนโครงสร้างเอกสาร.

{{% /alert %}}

## คุณสมบัติที่มีอยู่ในLowCodeAPI

เนมสเปซ`Aspose.Words.LowCode`รองรับในขณะนี้:

* **Converting**เอกสารจากรูปแบบหนึ่งไปยังอีก
* **Comparing**เอกสาร
* **Mail merging**
* **Reporting**ขึ้นอยู่กับLINQไวยากรณ์
* **Merging**เอกสาร
* **Search and replace**
* **Digital signing**ของเอกสาร
* **Splitting**เอกสารเป็นส่วนที่ใช้เกณฑ์ที่แตกต่างกัน
* การเพิ่ม**watermark**

{{% alert color="primary" %}}

โปรดทราบว่าคำอธิบายโดยละเอียดของแต่ละฟังก์ชั่นด้านนอกLow Codeสามารถพบได้ในส่วนคู่มือนักพัฒนาซอฟต์แวร์.

{{% /alert %}}

## คล่องแคล่วและไม่คล่องแคล่วAPI

Aspose.Wordsสำหรับ.NET รองรับทั้งคล่องแคล่วและไม่คล่องแคล่วAPIsช่วยให้นักพัฒนาที่จะเลือกรูปแบบที่เหมาะกับการ ลองดูตัวอย่างเพื่อดูว่าทั้งสองประเภทของAPIแตกต่างกันอย่างไร.

{{% alert color="primary" %}}

ในAPIคล่องแคล่ว,การดำเนินงานสามารถกำหนดค่าและดำเนินการผ่านบริบท(เช่นComparerContextหรือReplacerContext). บริบทนี้มีตัวเลือกทั่วไป รกำหนดค่าที่สอดคล้องกันทำให้APIมีประสิทธิภาพและง่ายต่อการจัดการในสถานการณ์ที่ซับซ้อ.

{{% /alert %}}

### เปรียบเทียบเอกสาร

ใช้`LowCode`เพื่อเปรียบเทียบเอกสารสองWordและบันทึกผลลัพธ์.

**ตัวอย่างที่ไม่คล่องแคล่ว:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.docx";
string outputDoc = "Compared.docx";

LowCodeComparer.Compare(firstDoc, secondDoc, outputDoc);
{{< /highlight >}}

**ตัวอย่างเช่น:**

{{< highlight csharp >}}
string firstDoc = "Document1.docx";
string secondDoc = "Document2.doc";

Comparer.Create()
   .From(firstDoc)
   .From(secondDoc)
   .To("CompareDocuments.1.docx")
   .Execute();
{{< /highlight >}}

คุณยังสามารถส่งผ่าน`CompareOptions`สำหรับการเปรียบเทียบอย่างละเอียด.

**ตัวอย่างที่ไม่คล่องแคล่ว:**

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

**ตัวอย่างเช่น:**

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

### แปลงเอกสารเป็นภาพ

ใช้`LowCode`เพื่อแปลงWordเอกสารเป็นPDF.

**ตัวอย่างที่ไม่คล่องแคล่ว:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Convert(inputDoc, outputDoc);
{{< /highlight >}}

**ตัวอย่างเช่น:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.pdf";

Converter.Create()
   .From(inputDoc)
   .To(outputDoc)
   .Execute();
{{< /highlight >}}

### ค้นหาและแทนที่ข้อความ

ใช้`LowCode`เพื่อแทนที่ข้อความในเอกสารทั้งหมดอย่างรวดเร็ว.

**ตัวอย่างที่ไม่คล่องแคล่ว:**

{{< highlight csharp >}}
string inputDoc = "Input.docx";
string outputDoc = "Output.docx";
string pattern = "Aspose";
string replacement = "Aspose Pro";

Replacer.Replace(inputDoc, outputDoc, pattern, replacement);
{{< /highlight >}}

**ตัวอย่างเช่น:**

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

## ทำไมต้องใช้Aspose.WordsLow Code

เนมสเปซ **Aspose.Words.LowCode** ช่วยให้คุณสามารถใช้งานการประมวลผลเอกสารระดับสูงได้อย่างรวดเร็วด้วยรูปแบบคำสั่งที่ชัดเจนและอ่านง่าย ซึ่งมีประโยชน์อย่างยิ่งสำหรับนักพัฒนาที่ต้องการความเร็ว ความเรียบง่าย และโค้ดที่บำรุงรักษาได้เมื่อทำงานกับเอกสาร Word.

ในการสำรวจตัวเลือกขั้นสูงมากขึ้นคุณสามารถรวมLowCodeAPIsกับรูปแบบวัตถุแบบเต็มAspose.Words ดูตัวอย่างเพิ่มเติมLow Codeใน[API documentation](https://reference.aspose.com/words/net/aspose.words.lowcode/).