---
title: การทำงานกับลายน้ำในC#
second_title: Aspose.Wordsสำหรับ.NET
articleTitle: การทำงานกับลายน้ำ
linktitle: การทำงานกับลายน้ำ
description: "การจัดการลายน้ำเอกสารโดยใช้C#."
type: docs
weight: 340
ai_search_scope: words_net
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /th/net/working-with-watermark/
timestamp: 2025-04-16-07-02-05
---

หัวข้อนี้กล่าวถึงวิธีการทำงานตามโปรแกรมด้วยลายน้ำโดยใช้Aspose.Words ลายน้ำเป็นภาพพื้นหลังที่แสดงอยู่เบื้องหลังข้อความในเอกสาร ลายน้ำสามารถประกอบด้วยข้อความหรือรูปภาพที่แสดงโดยคลาสของ[Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/).

{{% alert color="primary" %}}

**ลองออนไลน์**

คุณสามารถลองฟังก์ชั่นนี้กับเรา [ลายน้ำเอกสารออนไลน์ฟรี](https://products.aspose.app/words/watermark).

{{% /alert %}}

## เพิ่มลายน้ำในเอกสาร

ในMicrosoft Wordลายน้ำสามารถแทรกลงในเอกสารโดยใช้คำสั่งแทรกลายน้ำ Aspose.Wordsให้[watermark](https://reference.aspose.com/words/net/aspose.words/watermark/)คลาสที่จะเพิ่มหรือลบลายน้ำในเอกสาร. Aspose.Wordsให้การแจงนับ[WatermarkType](https://reference.aspose.com/words/net/aspose.words/watermark/type/)กำหนดสามประเภทที่เป็นไปได้ของลายน้ำ(ข้อความ,ภาพ,และไม่มี)ที่จะทำงา

### เพิ่มลายน้ำข้อความ

ตัวอย่างรหัสต่อไปนี้แสดงให้เห็นถึงวิธีการแทรกลายน้ำข้อความในเอกสารโดยการกำหนด[TextWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/textwatermarkoptions/)โดยใช้วิธีการ[SetText](https://reference.aspose.com/words/net/aspose.words/watermark/settext/#settext):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-text-watermark.cs" >}}

### เพิ่มลายน้ำภาพ

ตัวอย่างรหัสต่อไปนี้แสดงให้เห็นถึงวิธีการแทรกลายน้ำภาพในเอกสารโดยการกำหนด[ImageWatermarkOptions](https://reference.aspose.com/words/net/aspose.words/imagewatermarkoptions/)โดยใช้วิธีการ[SetImage](https://reference.aspose.com/words/net/aspose.words/watermark/setimage/#setimage):

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-image-watermark.cs" >}}

ลายน้ำภาพสามารถแทรกเป็นภาพสตริงหรือสตรีม.

ลายน้ำยังสามารถแทรกโดยใช้ชั้นเรียนรูปร่างได้เป็นอย่างดี มันเป็นเรื่องง่ายมากที่จะแทรกรูปร่างหรือภาพใดๆลงในส่วนหัวหรือส่วนท้ายและทำให้การส.

ตัวอย่างรหัสต่อไปนี้แทรกลงในเอกสารWord:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "add-document-watermark.cs" >}}

{{% alert color="primary" %}}

คุณสามารถดาวน์โหลดไฟล์ตัวอย่างของตัวอย่างนี้ได้จาก [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-.NET/blob/master/Examples/Data/Document.docx).

{{% /alert %}}


## ลบลายน้ำออกจากเอกสาร

คลาส[Watermark](https://reference.aspose.com/words/net/aspose.words/watermark/)มีวิธีการเอาออกเพื่อลบลายน้ำออกจากเอกสาร.

ตัวอย่างรหัสต่อไปนี้แสดงวิธีการลบลายน้ำจากเอกสาร:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-document-watermark.cs" >}}

หากมีการเพิ่มลายน้ำโดยใช้วัตถุระดับ[Shape](https://reference.aspose.com/words/net/aspose.words.drawing/shape/)จากนั้นในการลบลายน้ำออกจากเอกสารที่คุณต้องตั้งเฉพาะชื่อของรูปร่างลายน้ำในระหว่างการแทรกแล้วลบรูปร่างลายน้ำด้วยชื่อที่กำหนดไว้.

ตัวอย่างรหัสต่อไปนี้แสดงวิธีการตั้งค่าชื่อของรูปร่างลายน้ำและลบออกจากเอกสาร:

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "set-shape-name.cs" >}}

{{< gist "aspose-words-gists" "1f690a31c188a851d80d7aed4ff7e44c" "remove-watermark-shape.cs" >}}

## เพิ่มลายน้ำลงในเซลล์ตาราง

บางครั้งคุณต้องใส่ลายน้ำ/รูปภาพลงในเซลล์ของตารางและแสดงนอกโต๊ะคุณสามารถใช้คุณสมบัติ[IsLayoutInCell](https://reference.aspose.com/words/net/aspose.words.drawing/shapebase/islayoutincell/) คุณสมบัตินี้ได้รับหรือตั้งค่าสถานะที่ระบุว่ารูปร่างจะแสดงภายในตารางหรือภายนอกของมัน โปรดทราบว่าคุณสมบัตินี้ทำงานเฉพาะเมื่อคุณเพิ่มประสิทธิภาพเอกสารสำหรับMicrosoft Word2010 โดยใช้วิธี[OptimizeFor](https://reference.aspose.com/words/net/aspose.words.settings/compatibilityoptions/optimizefor/).

ตัวอย่างรหัสต่อไปนี้แสดงวิธีใช้คุณสมบัตินี้:

{{< gist "aspose-words-gists" "ad463bf5f128fe6e6c1485df3c046a4c" "layout-in-cell.cs" >}}
