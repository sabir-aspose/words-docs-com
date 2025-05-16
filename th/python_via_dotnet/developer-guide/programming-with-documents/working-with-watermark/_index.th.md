---
title: การทำงานกับลายน้ำในPython
second_title: Aspose.WordsสำหรับPython via .NET
articleTitle: การทำงานกับลายน้ำ
linktitle: การทำงานกับลายน้ำ
description: "สร้างและจัดการลายน้ำในเอกสารโดยใช้Python."
type: docs
weight: 340
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /th/python-net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

หัวข้อนี้กล่าวถึงวิธีการทำงานตามโปรแกรมด้วยลายน้ำโดยใช้Aspose.Words ลายน้ำเป็นภาพพื้นหลังที่แสดงอยู่เบื้องหลังข้อความในเอกสาร ลายน้ำสามารถประกอบด้วยข้อความหรือรูปภาพที่แสดงโดยคลาสของ[Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/).

{{% alert color="primary" %}}

**ลองออนไลน์**

คุณสามารถลองฟังก์ชั่นนี้กับเรา [ลายน้ำเอกสารออนไลน์ฟรี](https://products.aspose.app/words/watermark).

{{% /alert %}}

## วิธีการเพิ่มลายน้ำในเอกสาร

ในMicrosoft Wordลายน้ำสามารถแทรกลงในเอกสารโดยใช้คำสั่งแทรกลายน้ำ Aspose.Wordsมีชั้นเรียน[Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/)เพื่อเพิ่มหรือลบลายน้ำในเอกสาร Aspose.Wordsให้การแจงนับ[WatermarkType](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/)กำหนดสามประเภทที่เป็นไปได้ของลายน้ำ([TEXT](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#text),[IMAGE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#image)และ[NONE](https://reference.aspose.com/words/python-net/aspose.words/watermarktype/#none))ที่จะทำงานกับ.

### เพิ่มลายน้ำข้อความ

ตัวอย่างรหัสต่อไปนี้แสดงให้เห็นถึงวิธีการแทรกลายน้ำข้อความในเอกสารโดยการกำหนด[TextWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/textwatermarkoptions/)โดยใช้วิธีการ[set_text](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_text/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddTextWatermarkWithSpecificOptions.py" >}}

### เพิ่มลายน้ำภาพ

ตัวอย่างรหัสต่อไปนี้แสดงให้เห็นถึงวิธีการแทรกลายน้ำภาพในเอกสารโดยการกำหนด[ImageWatermarkOptions](https://reference.aspose.com/words/python-net/aspose.words/imagewatermarkoptions/)โดยใช้วิธีการ[set_image](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/):

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddImageWatermarkWithSpecificOptions.py" >}}

ลายน้ำภาพสามารถแทรกเป็นภาพสตริงหรือสตรีม.

ลายน้ำยังสามารถแทรกโดยใช้ชั้นเรียนรูปร่างได้เป็นอย่างดี มันเป็นเรื่องง่ายมากที่จะแทรกรูปร่างหรือภาพใดๆลงในส่วนหัวหรือส่วนท้ายและทำให้การส.

ตัวอย่างรหัสต่อไปนี้แทรกลงในเอกสารWord:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-AddWatermark.py" >}}

{{% alert color="primary" %}}

คุณสามารถดาวน์โหลดไฟล์แม่แบบของตัวอย่างนี้ได้จาก [ที่นี่](https://github.com/aspose-words/Aspose.Words-for-Python-via-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## ลบลายน้ำออกจากเอกสาร

คลาส[Watermark](https://reference.aspose.com/words/python-net/aspose.words/watermark/)มีวิธีการเอาออกเพื่อลบลายน้ำออกจากเอกสาร.

ตัวอย่างรหัสต่อไปนี้แสดงวิธีการลบลายน้ำจากเอกสาร:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermarkFromDocument.py" >}}

หากมีการเพิ่มลายน้ำโดยใช้วัตถุระดับ[Shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/)จากนั้นในการลบลายน้ำออกจากเอกสารที่คุณต้องตั้งเฉพาะชื่อของรูปร่างลายน้ำในระหว่างการแทรกแล้วลบรูปร่างลายน้ำด้วยชื่อที่กำหนดไว้.

ตัวอย่างรหัสต่อไปนี้แสดงวิธีการตั้งค่าชื่อของรูปร่างลายน้ำและลบออกจากเอกสาร:

{{< highlight python >}}
# Set name to be able to remove it afterwards
watermark.name = "WaterMark"
{{< /highlight >}}

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_watermark-RemoveWatermark.py" >}}

## เพิ่มลายน้ำในเซลล์ตาราง

บางครั้งคุณต้องใส่ลายน้ำ/รูปภาพลงในเซลล์ของตารางและแสดงนอกโต๊ะคุณสามารถใช้คุณสมบัติ[is_layout_in_cell](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/is_layout_in_cell/) คุณสมบัตินี้ได้รับหรือตั้งค่าสถานะที่ระบุว่ารูปร่างจะแสดงภายในตารางหรือภายนอกของมัน โปรดทราบว่าคุณสมบัตินี้ทำงานเฉพาะเมื่อคุณเพิ่มประสิทธิภาพเอกสารสำหรับMicrosoft Word2010 โดยใช้วิธี[optimize_for](https://reference.aspose.com/words/python-net/aspose.words.settings/compatibilityoptions/optimize_for/).

ตัวอย่างรหัสต่อไปนี้แสดงวิธีใช้คุณสมบัตินี้:

{{< gist "aspose-words-gists" "e9d8f984dac599756ccb4a64b8c79768" "Examples-DocsExamples-DocsExamples-Programming with Documents-Working with Graphic Elements-working_with_shapes-LayoutInCell.py" >}}
