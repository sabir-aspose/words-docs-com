---
title: แปลงเอกสารหลายหน้าเป็นรูปภาพในJava
second_title: Aspose.WordsสำหรับJava
articleTitle: แปลงเอกสารหลายหน้าเป็นรูปภาพ
linktitle: แปลงเอกสารหลายหน้าเป็นรูปภาพ
type: docs
description: "ส่งออกเอกสารหลายหน้าไปยังภาพแรสเตอร์(JPG, PNG, GIF, BMP, TIFF, WebP) ใช้Java."
weight: 37
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /th/java/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.WordsสำหรับJavaอนุญาตให้ผู้ใช้สามารถส่งออกเอกสารหลายหน้าไปยังภาพแรสเตอร์ การแสดงตัวอย่างเก็บถาวรหรือการแสดงภาพของเอกสารสำหรับการใช้งานที่ไม่สามาร.

## รูปแบบใดที่สนับสนุนการส่งออกหลายหน้า?

Aspose.Wordsรองรับการส่งออกหลายหน้าไปยังรูปแบบภาพแรสเตอร์ต่อไปนี้:

* เจพีอี
* อีเมล
* ปิงปอง
* บีเอ็มพี
* ทิฟฟ์
* WebP

## วิธีการส่งออกเอกสารหลายหน้าไปยังรูปภาพ

คุณลักษณะของการเอ็กซ์ปอร์ตเอกสารหลายหน้าไปยังรูปภาพถูกนำมาใช้โดยใช้คลาสของ[MultiPageLayout](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/)–คุณสามารถระบุวิธีการจัดระเบียบเพจเมื่อบันทึกลงในรูปภาพ:

* [SinglePage](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#singlePage)-บันทึกเฉพาะหน้าแรกที่ระบุ
* [Grid](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#grid-int-float-float)-จัดเรียงหน้าเว็บในตารางจากซ้ายไปขวาและจากบนลงล่างในขณะที่ระบุจำนวนคอลัมน์
* [Horizontal](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#horizontal-float)-จัดเรียงหน้าในแนวนอนด้านข้างซ้ายไปขวาในเอาต์พุตเดียว
* [Vertical](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#vertical-float)-จัดเรียงหน้าในแนวตั้งหนึ่งด้านล่างอื่นๆในผลลัพธ์เดียว
* [TiffFrames](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#tiffFrames)-จัดเรียงแต่ละหน้าเป็นเฟรมที่แยกต่างหากในภาพหลายเฟรมTIFFใช้ได้กับรูปแบบภาพTIFFเท่านั้น

ตัวอย่างรหัสต่อไปนี้แสดงวิธีการบันทึกเอกสารหลายหน้าDOCXเป็นภาพJPEGที่มีเค้าโครงแนวนอน:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.JPEG);
// Set up Horizontal layout.
options.setPageLayout = MultiPageLayout.Horizontal(10);

doc.save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

นอกจากนี้คุณยังสามารถปรับแต่งลักษณะที่ปรากฏของเพจไฟล์ที่ส่งออก–ระบุ[BackColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBackColor),[BorderColor](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderColor)และ[BorderWidth](https://reference.aspose.com/words/java/com.aspose.words/multipagelayout/#getBorderWidth).

ตัวอย่างรหัสต่อไปนี้แสดงวิธีการบันทึกเอกสารหลายหน้าDOCXเป็นPNGรูปภาพที่มีเค้าโครงตาราง:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.PNG);
// Set up a grid layout with:
// - 3 columns per row.
// - 10pts spacing between pages (horizontal and vertical).
options.setPageLayout(MultiPageLayout.grid(3, 10f, 10f));

// Customize the background and border.
options.getPageLayout().setBackColor(Color.lightGray);
options.getPageLayout().setBorderColor(Color.BLUE);
options.getPageLayout().setBorderWidth(2f);

doc.save("ImageSaveOptions.GridLayout.png", options);
{{< /highlight >}}