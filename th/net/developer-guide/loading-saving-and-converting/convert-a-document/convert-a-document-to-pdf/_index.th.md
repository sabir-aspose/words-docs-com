---
title: แปลง Word เป็น PDF ใน C#
second_title: Aspose.Words สำหรับ .NET
articleTitle: เปลี่ยนเอกสารเป็น PDF
linktitle: เปลี่ยนเอกสารเป็น PDF
description: "แปลง Word เป็น PDF ใน C# ตัวอย่างโค้ดง่ายๆ สำหรับการแปลง DOCX เป็น PDF รองรับทุกรูปแบบ Word และรูปภาพ"
type: docs
weight: 10
url: /th/net/convert-a-document-to-pdf/
timestamp: 2024-09-25-11-08-55
---

ความสามารถในการแปลงเอกสารอย่างง่ายดายและเชื่อถือได้จากรูปแบบหนึ่งไปยังอีกรูปแบบหนึ่งเป็นคุณสมบัติหลักของ Aspose.Words PDF เป็นหนึ่งในรูปแบบที่ได้รับความนิยมมากที่สุดสำหรับการแปลง – เป็นรูปแบบที่มีเค้าโครงแบบคงที่ที่รักษารูปลักษณ์เดิมของเอกสารไว้ระหว่างการแสดงผลบนแพลตฟอร์มต่างๆ คำว่า "การแสดงผล" ใช้ใน Aspose.Words เพื่ออธิบายกระบวนการแปลงเอกสารไปเป็นรูปแบบไฟล์ที่มีการแบ่งหน้าหรือมีแนวคิดเรื่องหน้า

## แปลงเอกสาร Word เป็น PDF

การแปลงจาก Word เป็น PDF เป็นกระบวนการที่ค่อนข้างซับซ้อนซึ่งต้องใช้หลายขั้นตอนของการคำนวณ เอนจินการจัดวางของ Aspose.Words เลียนแบบวิธีการทำงานของเอนจินการจัดวางหน้าของ Microsoft Word ทำให้เอกสาร PDF ที่ส่งออกมาดูใกล้เคียงกับสิ่งที่คุณเห็นใน Microsoft Word มากที่สุด

ด้วย Aspose.Words คุณสามารถเปลี่ยนเอกสารโดยทางโปรแกรมจากรูปแบบ Word เช่น DOC หรือ DOCX เป็น PDF โดยไม่ต้องใช้ Microsoft Office บทความนี้อธิบายวิธีการแปลงรูปแบบนี้

{{% alert color="primary" %}}

โปรดทราบว่าจำนวนหน้าในเอกสารจะส่งผลต่อเวลาในการแปลง

{{% /alert %}}

### แปลง DOCX หรือ DOC เป็น PDF

การเปลี่ยนจากรูปแบบเอกสาร DOC หรือ DOCX เป็นรูปแบบ PDF ใน Aspose.Words นั้นง่ายมากและสามารถทำได้ด้วยโค้ดเพียงสองบรรทัดที่:

1. โหลดเอกสารของคุณลงในออบเจกต์ [Document](https://reference.aspose.com/words/net/aspose.words/document/) โดยใช้คอนสตรัคเตอร์ใดตัวหนึ่งโดยระบุชื่อเอกสารพร้อมนามสกุลรูปแบบ
1. เรียกใช้เมธอด [Document.Save](https://reference.aspose.com/words/net/aspose.words/document/save/#save/) หนึ่งในหลายตัวบนออบเจกต์ **Document** และระบุรูปแบบเอาต์พุตที่ต้องการเป็น PDF โดยป้อนชื่อไฟล์ที่มีนามสกุล ".PDF"

ตัวอย่างโค้ดต่อไปนี้แสดงวิธีการแปลงเอกสารจาก DOCX เป็น PDF โดยใช้เมธอด [Save](https://reference.aspose.com/words/net/aspose.words/document/save/):

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "docx-to-pdf.cs" >}}

คุณสามารถดาวน์โหลดไฟล์เทมเพลตของตัวอย่างนี้ได้จาก [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Rendering.docx)

{{% alert color="primary" %}}

บางครั้งจำเป็นต้องระบุตัวเลือกเพิ่มเติมที่อาจส่งผลต่อผลลัพธ์ของการบันทึกเอกสารเป็น PDF ตัวเลือกเหล่านี้สามารถระบุได้โดยใช้คลาส [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) ซึ่งมีคุณสมบัติที่กำหนดวิธีการแสดงเอาต์พุต PDF

โปรดทราบว่าด้วยเทคนิคเดียวกัน คุณสามารถเปลี่ยนเอกสารรูปแบบ flow-layout ใดๆ ไปเป็นรูปแบบ PDF ได้

{{% /alert %}}

### แปลงแบบเป็นมาตรฐาน PDF ต่างๆ

Aspose.Words มี enumeration [PdfCompliance](https://reference.aspose.com/words/net/aspose.words.saving/pdfcompliance/) เพื่อสนับสนุนการแปลง DOC หรือ DOCX เป็นมาตรฐานรูปแบบ PDF ต่างๆ (เช่น PDF 1.7, PDF 1.5 เป็นต้น)

ตัวอย่างโค้ดต่อไปนี้แสดงวิธีการแปลงเอกสารเป็น PDF 1.7 โดยใช้ [PdfSaveOptions](https://reference.aspose.com/words/net/aspose.words.saving/pdfsaveoptions/) ที่สอดคล้องกับ PDF17:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "conversion-to-pdf17.cs" >}}

## แปลงรูปภาพเป็น PDF

การแปลงเป็น PDF ไม่ได้จำกัดเฉพาะรูปแบบเอกสาร Microsoft Word เท่านั้น รูปแบบใดๆ ที่สนับสนุนโดย Aspose.Words รวมถึงที่สร้างขึ้นโดยทางโปรแกรม ก็สามารถเปลี่ยนเป็น PDF ได้เช่นกัน ตัวอย่างเช่น เราสามารถแปลงรูปภาพหน้าเดียว เช่น JPEG, PNG, BMP, EMF หรือ WMF รวมถึงรูปภาพหลายหน้า เช่น TIFF และ GIF เป็น PDF

ตัวอย่างโค้ดต่อไปนี้แสดงวิธีการเปลี่ยนรูปภาพ JPEG และ TIFF เป็น PDF:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "image-to-pdf.cs" >}}

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "convert-image-to-pdf.cs" >}}

เพื่อให้โค้ดนี้ทำงานได้ คุณจำเป็นต้องเพิ่มการอ้างอิงไปยัง Aspose.Words และ `System.Drawing` ในโปรเจกต์ของคุณ

## ลดขนาดเอาต์พุต PDF

เมื่อบันทึกเป็น PDF คุณสามารถระบุได้ว่าต้องการปรับปรุงเอาต์พุตหรือไม่ ในการทำเช่นนี้ คุณจำเป็นต้องตั้งค่าแฟล็ก [OptimizeOutput](https://reference.aspose.com/words/net/aspose.words.saving/fixedpagesaveoptions/optimizeoutput/) เป็น true และแล้วแคนวาสที่ซ้อนกันและว่างเปล่าที่ซ้ำซ้อนจะถูกลบออก กลิฟที่อยู่ติดกันซึ่งมีการจัดรูปแบบเหมือนกันจะถูกรวมกัน

ตัวอย่างโค้ดต่อไปนี้แสดงวิธีการปรับปรุงเอาต์พุต:

{{< gist "aspose-words-gists" "a53bdaad548845275c1b9556ee21ae65" "optimize-output.cs" >}}

{{% alert color="primary" %}}

การใช้คุณสมบัติ **OptimizeOutput** อาจส่งผลต่อความแม่นยำของการแสดงเนื้อหา

{{% /alert %}}

## ดูเพิ่มเติม

- บทความ [การแสดงผล](/words/th/net/rendering/) สำหรับข้อมูลเพิ่มเติมเกี่ยวกับรูปแบบหน้าคงที่และการจัดวางแบบโฟลว์
- บทความ [การแปลงเป็นรูปแบบหน้าคงที่](/words/net/converting-to-fixed-page-format/#what-is-a-page-layout) สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการจัดวางหน้า
- บทความ [ระบุตัวเลือกการแสดงผลเมื่อแปลงเป็น PDF](/words/th/net/specify-rendering-options-when-converting-to-pdf/) สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการใช้คลาส `PdfSaveOptions`
- บทความ [เรียนรู้คุณสมบัติของการแปลงเป็น PDF/A และ PDF/UA](/words/th/net/learn-features-of-conversion-to-pdf-a-pdf-ua/) ที่อธิบายว่ามาตรฐาน PDF ใดและ ISO ที่เกี่ยวข้องสำหรับมาตรฐาน PDF ที่สนับสนุนโดย Aspose.Words
- บทความ [มาตรฐาน PDF ใดดีกว่าที่จะเลือก](/words/th/net/which-pdf-standard-is-better-to-choose/) เพื่อกำหนดว่ามาตรฐาน PDF ใดเหมาะสมกับกรณีใด

- บทความ [การทำงานกับ PDF/A หรือ PDF/UA](/words/th/net/working-with-pdfa-or-pdfua/) อธิบายข้อกำหนดสำหรับเนื้อหาเอกสารในรูปแบบ PDF/A และ PDF/UA – ส่วนใหญ่เป็นข้อกำหนดสำหรับโครงสร้างและแบบอักษร

- บทความ [คำเตือนปัญหาการเข้าถึงเมื่อบันทึกเป็น PDF/A และ PDF/UA](/words/th/net/warnings-when-saving-to-pdfa-and-pdfua/) อธิบายว่าข้อกำหนดการเข้าถึงเนื้อหาใดที่ PDF/A และ PDF/UA กำหนดไว้
