---
title: แปลงเอกสารหลายหน้าเป็นรูปภาพในC#
second_title: Aspose.Wordsสำหรับ.NET
articleTitle: แปลงเอกสารหลายหน้าเป็นรูปภาพ
linktitle: แปลงเอกสารหลายหน้าเป็นรูปภาพ
type: docs
description: "ส่งออกเอกสารหลายหน้าไปยังภาพแรสเตอร์(JPG, PNG, GIF, BMP, TIFF, WebP) ใช้C#."
weight: 44
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /th/net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.Wordsสำหรับ.NETอนุญาตให้ผู้ใช้สามารถส่งออกเอกสารหลายหน้าไปยังภาพแรสเตอร์ การแสดงตัวอย่างเก็บถาวรหรือการแสดงภาพของเอกสารสำหรับการใช้งานที่ไม่สามาร.

## รูปแบบใดที่สนับสนุนการส่งออกหลายหน้า?

Aspose.Wordsรองรับการส่งออกหลายหน้าไปยังรูปแบบภาพแรสเตอร์ต่อไปนี้:

* เจพีอี
* อีเมล
* ปิงปอง
* บีเอ็มพี
* ทิฟฟ์
* WebP

## วิธีการส่งออกเอกสารหลายหน้าไปยังรูปภาพ

คุณลักษณะของการเอ็กซ์ปอร์ตเอกสารหลายหน้าไปยังรูปภาพถูกนำมาใช้โดยใช้คลาสของ[MultiPageLayout](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/)–คุณสามารถระบุวิธีการจัดระเบียบเพจเมื่อบันทึกลงในรูปภาพ:

* [SinglePage](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/singlepage/)-บันทึกเฉพาะหน้าแรกที่ระบุ
* [Grid](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/grid/)-จัดเรียงหน้าเว็บในตารางจากซ้ายไปขวาและจากบนลงล่างในขณะที่ระบุจำนวนคอลัมน์
* [Horizontal](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/horizontal/)-จัดเรียงหน้าในแนวนอนด้านข้างซ้ายไปขวาในเอาต์พุตเดียว
* [Vertical](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/vertical/)-จัดเรียงหน้าในแนวตั้งหนึ่งด้านล่างอื่นๆในผลลัพธ์เดียว
* [TiffFrames](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/tiffframes/)-จัดเรียงแต่ละหน้าเป็นเฟรมที่แยกต่างหากในภาพหลายเฟรมTIFFใช้ได้กับรูปแบบภาพTIFFเท่านั้น

ตัวอย่างรหัสต่อไปนี้แสดงวิธีการบันทึกเอกสารหลายหน้าDOCXเป็นภาพJPEGที่มีเค้าโครงแนวนอน:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Jpeg);
// Set up Horizontal layout.
options.PageLayout = MultiPageLayout.Horizontal(10);

doc.Save("ImageSaveOptions.HorizontalLayout.jpg", options);
{{< /highlight >}}

นอกจากนี้คุณยังสามารถปรับแต่งลักษณะที่ปรากฏของเพจไฟล์ที่ส่งออก–ระบุ[BackColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/backcolor/),[BorderColor](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/bordercolor/)และ[BorderWidth](https://reference.aspose.com/words/net/aspose.words.saving/multipagelayout/borderwidth/).

ตัวอย่างรหัสต่อไปนี้แสดงวิธีการบันทึกเอกสารหลายหน้าDOCXเป็นPNGรูปภาพที่มีเค้าโครงตาราง:

{{< highlight csharp >}}
Document doc = new Document("Rendering.docx");

ImageSaveOptions options = new ImageSaveOptions(SaveFormat.Png);
// Set up a grid layout with:
// - 3 columns per row.
// - 10pts spacing between pages (horizontal and vertical).
options.PageLayout = MultiPageLayout.Grid(3, 10, 10);

// Customize the background and border.
options.PageLayout.BackColor = Color.LightGray;
options.PageLayout.BorderColor = Color.Blue;
options.PageLayout.BorderWidth = 2;

doc.Save("ImageSaveOptions.GridLayout.png", options);
{{< /highlight >}}