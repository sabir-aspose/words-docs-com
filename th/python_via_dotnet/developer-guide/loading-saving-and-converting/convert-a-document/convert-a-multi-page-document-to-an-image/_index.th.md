---
title: แปลงเอกสารหลายหน้าเป็นรูปภาพในPython
second_title: Aspose.WordsสำหรับPython
articleTitle: แปลงเอกสารหลายหน้าเป็นรูปภาพ
linktitle: แปลงเอกสารหลายหน้าเป็นรูปภาพ
type: docs
description: "ส่งออกเอกสารหลายหน้าไปยังภาพแรสเตอร์(JPG, PNG, GIF, BMP, TIFF, WebP) ใช้Python."
weight: 44
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /th/python-net/convert-a-multi-page-document-to-an-image/
timestamp: 2025-06-18-10-00-04
---

Aspose.WordsสำหรับPython via .NETอนุญาตให้ผู้ใช้สามารถส่งออกเอกสารหลายหน้าไปยังภาพแรสเตอร์ การแสดงตัวอย่างเก็บถาวรหรือการแสดงภาพของเอกสารสำหรับการใช้งานที่ไม่สามาร.

## รูปแบบใดที่สนับสนุนการส่งออกหลายหน้า?

Aspose.Wordsรองรับการส่งออกหลายหน้าไปยังรูปแบบภาพแรสเตอร์ต่อไปนี้:

* เจพีอี
* อีเมล
* ปิงปอง
* บีเอ็มพี
* ทิฟฟ์
* WebP

## วิธีการส่งออกเอกสารหลายหน้าไปยังรูปภาพ

คุณลักษณะของการเอ็กซ์ปอร์ตเอกสารหลายหน้าไปยังรูปภาพถูกนำมาใช้โดยใช้คลาสของ[MultiPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/)–คุณสามารถระบุวิธีการจัดระเบียบเพจเมื่อบันทึกลงในรูปภาพ:

* [single_page](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/single_page/)-บันทึกเฉพาะหน้าแรกที่ระบุ
* [grid](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/grid/#int_float_float)-จัดเรียงหน้าเว็บในตารางจากซ้ายไปขวาและจากบนลงล่างในขณะที่ระบุจำนวนคอลัมน์
* [horizontal](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/horizontal/#float)-จัดเรียงหน้าในแนวนอนด้านข้างซ้ายไปขวาในเอาต์พุตเดียว
* [vertical](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/vertical/#float)-จัดเรียงหน้าในแนวตั้งหนึ่งด้านล่างอื่นๆในผลลัพธ์เดียว
* [tiff_frames](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/tiff_frames/)-จัดเรียงแต่ละหน้าเป็นเฟรมที่แยกต่างหากในภาพหลายเฟรมTIFFใช้ได้กับรูปแบบภาพTIFFเท่านั้น

ตัวอย่างรหัสต่อไปนี้แสดงวิธีการบันทึกเอกสารหลายหน้าDOCXเป็นภาพJPEGที่มีเค้าโครงแนวนอน:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.JPEG)
# Set up Horizontal layout.
options.page_layout = MultiPageLayout.Horizontal(10);

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}

นอกจากนี้คุณยังสามารถปรับแต่งลักษณะที่ปรากฏของเพจไฟล์ที่ส่งออก–ระบุ[back_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/back_color/),[border_color](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_color/)และ[border_width](https://reference.aspose.com/words/python-net/aspose.words.saving/multipagelayout/border_width/).

ตัวอย่างรหัสต่อไปนี้แสดงวิธีการบันทึกเอกสารหลายหน้าDOCXเป็นPNGรูปภาพที่มีเค้าโครงตาราง:

{{< highlight csharp >}}
doc = aw.Document(file_name='Rendering.docx')

options = aw.saving.ImageSaveOptions(aw.SaveFormat.PNG)
# Set up a grid layout with:
# - 3 columns per row.
# - 10pts spacing between pages (horizontal and vertical).
options.page_layout = aw.saving.MultiPageLayout.grid(3, 10, 10)

# Customize the background and border.
options.page_layout.back_color = aspose.pydrawing.Color.light_gray
options.page_layout.border_color = aspose.pydrawing.Color.blue
options.page_layout.border_width = 2

doc.save(file_name='ImageSaveOptions.GridLayout.jpg', save_options=options)
{{< /highlight >}}