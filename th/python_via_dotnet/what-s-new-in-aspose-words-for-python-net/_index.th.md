---
title: มีอะไรใหม่
second_title: Aspose.WordsสำหรับPython via .NET
articleTitle: มีอะไรใหม่ใน Aspose.WordsสำหรับPython via .NET
linktitle: มีอะไรใหม่ใน Aspose.WordsสำหรับPython via .NET
type: docs
description: "Aspose.WordsสำหรับPython via .NET ขยายและปรับปรุงทุกวัน ในหน้านี้คุณสามารถเรียนรู้เกี่ยวกับคุณสมบัติขนาดใหญ่และน่าสนใจที่สุดของผลิตภัณฑ์."
weight: 10
ai_search_scope: words_python
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /th/python-net/what-s-new-in-aspose-words-for-python-net/
timestamp: 2025-04-16-07-02-05
---

หน้านี้อธิบายถึงคุณลักษณะใหม่ที่น่าสนใจที่สุดAspose.Wordsที่นำมาใช้ในรุ่นล่าสุด.

## Aspose.Words สำหรับ Python ผ่านทาง .NET 25.1, 25.2, 25.3, 25.4

Aspose.Words25.1แนะนำการตรวจสอบไวยากรณ์ที่ขับเคลื่อนAIและเพิ่มการประหยัดเอกสารด้วยตัวเลือกขั้นสูงสำหรับHTML,SVGและMarkdownรูปแบบ.

Aspose.Words25.2นำเสนอการสรุปข้อความด้วยAnthropicAIรุ่น,เพิ่มMsWorksสนับสนุนรูปแบบ,เพิ่มการควบคุมการพิมพ์,และปรับปรุงPDFโครงสร้างและการจัดการรายการ.

Aspose.Words25.3ช่วยเพิ่มตัวตรวจสอบไวยากรณ์ที่ขับเคลื่อนAIและการเลือกแบบอักษรด้วยคุณสมบัติUpdateAmbiguousTextFontรวมทั้งช่วยเพิ่มการส่งออกไฟล์แนบPDF.

Aspose.Words25.4แนะนำการสนับสนุนสำหรับขนาดกระดาษใหม่ช่วยให้สามารถควบคุมการส่งออกขั้นสูงHTMLและปรับปรุงการจัดการลายน้ำ.

### AI-คุณสมบัติขับเคลื่อน

#### เอกสารAIการตรวจสอบไวยากรณ์

* ความสามารถในการตรวจสอบไวยากรณ์ของเอกสารที่ให้ไว้โดยใช้OpenAIรุ่นกำเนิดได้รับการแนะนำโดยการเพิ่มวิธีการ[check_grammar](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/check_grammar/)ใหม่ <sup>25.1</sup>
* คุณลักษณะการตรวจสอบไวยากรณ์แบบAIได้รับการอัปเดตเพื่อรองรับทุกรุ่นที่มีอยู่ในการแจงนับ[AiModelType](https://reference.aspose.com/words/python-net/aspose.words.ai/aimodeltype/) <sup>25.3</sup>

#### การสรุปโดยใช้แบบจำลองภาษาสร้างAnthropic <sup>25.2</sup>

การสรุปข้อความโดยใช้แบบจำลองภาษาสร้างAnthropicถูกเปิดใช้งานโดยการแนะนำชั้นเรียนสาธารณะใหม่[AnthropicAiModel](https://reference.aspose.com/words/python-net/aspose.words.ai/anthropicaimodel/).

### รูปแบบที่รองรับ <sup>25.2</sup>

เริ่มต้นจากรุ่น25.2มีการเพิ่มความเข้ากันได้กับรูปแบบใหม่MsWorksโหลดสำหรับMicrosoftเอกสารงาน.

### การแปลงโหลดและบันทึกเอกสาร

#### ปรับปรุงการประหยัดเป็นHTMLและSVGรูปแบบ <sup>25.1</sup>

การบันทึกไปยังHTMLและSVGรูปแบบได้รับการปรับปรุงโดยการเพิ่ม**id_prefix**และ**remove_java_script_from_links**คุณสมบัติทั้ง[HtmlFixedSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlfixedsaveoptions/)และ[SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/)คลาส.

#### ตั้งค่าความละเอียดของภาพและOfficeMathโหมดเอาท์พุทเมื่อบันทึกเป็นMarkdown <sup>25.1</sup>

* มีการเพิ่มตัวเลือก[image_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/image_resolution/)ใหม่ในชั้นเรียน[MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/)เพื่อตั้งค่าความละเอียดของภาพ.
* ตัวเลือกใหม่[office_math_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/office_math_export_mode/)และ[MarkdownOfficeMathExportMode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownofficemathexportmode/)การแจงนับได้รับและเพิ่มในชั้นเรียน[MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/)เพื่อตั้งOfficeMathโหมดเอาท์พุท.

### การแสดงผล

#### ปรับปรุงการควบคุมการพิมพ์ <sup>25.2</sup>

มีการเพิ่มคุณสมบัติ[number_spacing](https://reference.aspose.com/words/python-net/aspose.words/font/number_spacing/)เพื่อปรับปรุงการควบคุมการพิมพ์.

#### การควบคุมการเลือกแบบอักษรสำหรับตัวอักษรที่ไม่ชัดเจน <sup>25.3</sup>

คุณสมบัติสาธารณะใหม่[update_ambiguous_text_font](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/update_ambiguous_text_font/)ถูกเพิ่มในชั้นเรียน[SaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/saveoptions/)เพื่อควบคุมการเลือกแบบอักษรตามรหัสอักขระที่ใช้.

#### ตัวเลือกขนาดกระดาษ <sup>25.4</sup>

ความสามารถในการใช้JISB4และJISB5ขนาดกระดาษได้รับการแนะนำโดยการเพิ่มค่าใหม่ในการแจงนับ[PaperSize](https://reference.aspose.com/words/python-net/aspose.words/papersize/).

#### HTMLการควบคุมเอาท์พุท <sup>25.4</sup>

ความสามารถในการลบJavaScriptจากการเชื่อมโยงหลายมิติURLsระหว่างการส่งออกHTMLได้รับการแนะนำโดยการเพิ่มคุณสมบัติ[RemoveJavaScriptFromLinks](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/remove_java_script_from_links/).

### อื่นๆ

* PDFโครงสร้างตรรกะได้รับการปรับปรุงด้วยการสนับสนุนสำหรับฟิลด์TOA,BIBLIOGRAPHYและINDEX <sup>25.2</sup>
* วิธีการ[add_single_level_list](https://reference.aspose.com/words/python-net/aspose.words.lists/listcollection/add_single_level_list/#listtemplate)ได้รับการแนะนำสำหรับการจัดการรายการที่ดีขึ้น <sup>25.2</sup>
* มีการเพิ่มคุณสมบัติใหม่[attachments_embedding_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/attachments_embedding_mode/)เพื่อแทนที่**EmbedAttachments**เพื่อปรับปรุงการส่งออกสิ่งที่แนบมาPDF นอกจากนี้ยังมีการเพิ่มค่าใหม่ในการแจงนับ[PdfCompliance](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfcompliance/)เพื่อรองรับสิ่งที่แนบรุ่นPDF/A นอกจากนี้สิ่งที่แนบมาได้รับการสนับสนุนด้วยการเข้ารหัส <sup>25.3</sup>
* ความสามารถในการตั้งลายน้ำภาพจากกระแสได้รับการแนะนำโดยการเพิ่มโอเวอร์โหลดใหม่ให้กับวิธีการ[SetImage](https://reference.aspose.com/words/python-net/aspose.words/watermark/set_image/#bytesio_imagewatermarkoptions) <sup>25.4</sup>

{{% alert color="primary" %}}

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 25.1บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-1-release-notes/).

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 25.2บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-2-release-notes/).

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 25.3บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2025/aspose-words-for-python-via-dotnet-25-3-release-notes/).

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 25.4บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-25-4-release-notes/).

{{% /alert %}}

## Aspose.Words สำหรับ Python ผ่านทาง .NET 24.9, 24.10, 24.11, 24.12

Aspose.Words24.9แนะนำการแทรกgroup shapeและการแทรกStructuredDocumentTagผ่านทางDocumentBuilderช่วยเพิ่มการแสดงผลแผนภูมิรัศมีด้วยการสำเร็จการศึกษาปรับปรุงลายเซ็นดิจิตอลด้วยการสนับสนุนXAdES-EPESเพิ่มการรับรู้ขีดเส้นใต้Markdownและให้การเข้าถึงเชิงอรรถ/ตัวคั่นปลายทาง.

Aspose.Words24.10แนะนำการสนับสนุนการควบคุมที่เพิ่มขึ้นActiveXด้วยการสร้างCommandButtonการควบคุมการมองเห็นรูปร่างใหม่ความสามารถในการgroup shapesปรับปรุงMarkdownการส่งออกสำหรับตาราง,การจัดรูปแบบแผนภูมิสำหรับPieและDoughnutการจัดการการเข้ารหัสขนาดใหญ่ที่ดีขึ้นและการสนับสนุนสำหรับแบบอักษรที่ล้าสมัยของไต้หวัน.

Aspose.Words24.11แนะนำการสรุปเอกสารที่ขับเคลื่อนAIตัวเลือกการแสดงผลที่เพิ่มขึ้นการเข้าถึงคุณสมบัติของเอกสารที่ดีขึ้นและคำอธิบายการควบคุมActiveX.

Aspose.Words24.12แนะนำการจัดวางฉลากข้อมูลที่ปรับแต่งได้,กูเกิลAIแปลข้อความ,และเพิ่มชั้นเรียนการประมวลผลใหม่LowCode.

### AI-คุณสมบัติขับเคลื่อน

#### การสรุปเอกสารโดยใช้OpenAIและกูเกิล <sup>24.11</sup>

มีการบูรณาการการสนับสนุนสำหรับการสรุปเอกสารโดยใช้โมเดลภาษากำเนิด **OpenAI** และ **Google** โดยการเพิ่มเนมสเปซ [Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/) เข้ากับเมมเบอร์สาธารณะ.

#### แปลข้อความโดยใช้แบบจำลองภาษาที่สร้างขึ้นของกูเกิล <sup>24.12</sup>

ได้ถูกนำมาใช้ในAspose.Wordsโดยการเพิ่มวิธีการ[translate](https://reference.aspose.com/words/python-net/aspose.words.ai/iaimodeltext/translate/)และการแจงนับ[Language](https://reference.aspose.com/words/python-net/aspose.words.ai/language/)ไปยังเนมสเปซ[Aspose.Words.AI](https://reference.aspose.com/words/python-net/aspose.words.ai/).

### Low Code <sup>24.12</sup>

ใหม่LowCodeชั้นเรียนเช่น[Comparer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/comparer/), [MailMerger](https://reference.aspose.com/words/python-net/aspose.words.lowcode/mailmerger/), [Replacer](https://reference.aspose.com/words/python-net/aspose.words.lowcode/replacer/), [Splitter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/splitter/) ฯลฯ ได้รับการแนะนำนำเสนอชุดของวิธีการที่สมดุลที่สมบูรณ์แบบระหว่างความเรียบง่ายและ.

### การแสดงผลและการพิมพ์

#### จบการศึกษาในแผนภูมิรัศมี <sup>24.9</sup>

การแสดงผลของการสำเร็จการศึกษาในแผนภูมิรัศมีได้รับการดำเนินการ.

#### CommandButtonActiveXการควบคุม <sup>24.10</sup>

ความสามารถในการสร้างCommandButtonActiveXตัวควบคุมได้รับการแนะนำโดยการเพิ่มวิธีการสาธารณะใหม่[insert_forms_2_ole_control](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_forms_2_ole_control/)และชั้นเรียนสาธารณะใหม่[Forms2OleControl](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/).

#### ควบคุมการมองเห็นรูปร่าง <sup>24.10</sup>

มีการเพิ่มคุณสมบัติสาธารณะใหม่[hidden](https://reference.aspose.com/words/python-net/aspose.words.drawing/shapebase/hidden/)เพื่อควบคุมการมองเห็นของรูปร่าง.

#### การเปลี่ยนแปลงในPieและDoughnutแผนภูมิ <sup>24.10</sup>

คุณสมบัติสาธารณะใหม่หลายแห่งถูกเพิ่มลงในรูปแบบPieและDoughnutแผนภูมิ.

#### ควบคุมการแสดงผลของPDFเส้นขอบเขตฟิลด์ฟอร์มทางเลือก <sup>24.11</sup>

อ็อพชันใหม่ในการควบคุมการแสดงผลของPDFเส้นขอบเขตของฟิลด์ฟอร์มทางเลือกถูกนำมาใช้โดยการเพิ่มอ็อพชันพับลิกใหม่[render_choice_form_field_border](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/render_choice_form_field_border/).

#### รับและตั้งค่ารหัสรูปแบบสำหรับข้อมูลแผนภูมิ <sup>24.11</sup>

มีการเพิ่มความสามารถในการรับและตั้งค่ารหัสรูปแบบสำหรับข้อมูลแผนภูมิโดยการใช้[format_code](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/format_code/)คุณสมบัติในชั้นเรียน[ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/),[ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/)และ[BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/).

#### แสดงกราฟฮิสโตแกรมที่มีถังขยะและป้ายกำกับ <sup>24.11</sup>

การแสดงผลแผนภูมิฮิสโตแกรมได้รับการปรับปรุงโดยการอนุญาตให้จำนวนที่ระบุของถัง.

#### กำหนดตำแหน่งของป้ายกำกับข้อมูลเอง <sup>24.12</sup>

ความสามารถในการกำหนดตำแหน่งของป้ายชื่อข้อมูลได้ถูกเพิ่มโดยการแนะนำคุณสมบัติใหม่ให้กับชั้นเรียนชั้นที่[ChartDataLabel](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabel/)และ[ChartDataLabelCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatalabelcollection/).

### การแปลงโหลดและบันทึกเอกสาร

#### ขีดเส้นใต้การจัดรูปแบบเมื่อโหลดไฟล์Markdown <sup>24.9</sup>

ตัวเลือกในการจดจำการจัดรูปแบบขีดเส้นใต้เมื่อโหลดเอกสารMarkdownได้ถูกรวมไว้โดยการเพิ่มคุณสมบัติสาธารณะใหม่[import_underline_formatting property](https://reference.aspose.com/words/python-net/aspose.words.loading/markdownloadoptions/import_underline_formatting/).

#### ส่งออกตารางเป็นHTMLเมื่อบันทึกเป็นMarkdown <sup>24.10</sup>

ตัวเลือกในการส่งออกตารางเป็นHTMLเมื่อมีการบันทึกเอกสารไปยังรูปแบบMarkdownโดยการเพิ่มคุณสมบัติสาธารณะใหม่[export_as_html](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/export_as_html/)และการแจงนับ[MarkdownExportAsHtml](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownexportashtml/).

#### ส่งออกPDFด้วยโครงสร้างตรรกะที่ปรับปรุงแล้ว <sup>24.11</sup>

PDFเอ็กซ์ปอร์ตได้รับการปรับปรุงโดยรวมคุณสมบัติชื่อตารางเป็นชื่อองค์ประกอบโครงสร้างตรรกะPDF.

### ลายเซ็นดิจิตอล

#### ลงนามในเอกสารด้วยXAdES-EPES <sup>24.9</sup>

ความสามารถในการลงนามในเอกสารด้วยXAdES-EPESระดับXML-DSigลายเซ็นได้รับการแนะนำโดยการเพิ่มสถานที่ให้บริการสาธารณะใหม่[xml_dsig_level](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/signoptions/xml_dsig_level/)และการแจงนับสาธารณะใหม่[XmlDsigLevel](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/xmldsiglevel/).

### อื่นๆ

* วิธีการสาธารณะใหม่[insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/)ถูกเพิ่มเข้าไปgroup shapes <sup>24.9</sup>
* มีการเพิ่มวิธีการสาธารณะใหม่[insert_structured_document_tag](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_structured_document_tag/)เพื่อแทรก**StructuredDocumentTags**ลงในเอกสาร <sup>24.9</sup>
* การเข้าถึงสาธารณะเพื่อแยกเชิงอรรถ/สิ้นสุดหมายเหตุได้รับการให้บริการโดยการเพิ่มชั้ <sup>24.9</sup>
* ความสามารถในการจัดกลุ่มรูปร่างของแต่ละบุคคลgroup shapesเข้าด้วยกันและจัดกลุ่มโดยตรงทั้งรูปร่างและgroup shapesได้รับการแนะนำโดยการเพิ่มวิธีการ[insert_group_shape](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_group_shape/#float_float_float_float_shapebaselist) <sup>24.10</sup>
* การจัดการการเข้ารหัสขนาดใหญ่ 5 สำหรับTrueTypeตารางซีแมปได้รับการปรับปรุง <sup>24.10</sup>
* การสนับสนุนสำหรับแบบอักษรไต้หวันล้าสมัยได้รับการปรับปรุง <sup>24.10</sup>
* เพื่อเข้าถึงคุณสมบัติเอกสารขยาย คุณสมบัติแบบอ่านอย่างเดียวได้รับการเพิ่มลงในคลาส [BuiltInDocumentProperties](https://reference.aspose.com/words/python-net/aspose.words.properties/builtindocumentproperties/) แล้ว <sup>24.11</sup>
* การตั้งค่าคำบรรยายสำหรับActiveXมีการเปิดใช้งานโดยการเพิ่มตัวตั้งค่าพับลิกใหม่ในคุณสมบัติ[Forms2OleControl.caption](https://reference.aspose.com/words/python-net/aspose.words.drawing.ole/forms2olecontrol/caption/) <sup>24.11</sup>

{{% alert color="primary" %}}

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 24.9บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-9-release-notes/).

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 24.10บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-10-release-notes/).

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 24.11บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-11-release-notes/).

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 24.12บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-12-release-notes/).

{{% /alert %}}

## Aspose.Words สำหรับ Python ผ่านทาง .NET 24.5, 24.6, 24.7, 24.8

Aspose.Words24.5ขยายตัวเลือกสำหรับแอสเซมบลีปรับปรุงความสามารถในการแสดงผลและขยายตัวเลือกอื่นๆ.

Aspose.Words24.6ปรับปรุงตัวเลือกการแสดงผลเพิ่มการค้นหาและเปรียบเทียบฟังก์ชันการทำงานและขย.

Aspose.Words24.7เปลี่ยนวิธีการทำงานกับActiveXขยายความสามารถในการแสดงผลตลอดจนการส่งออกไปยังMarkdownและXLSXรูปแบบ.

Aspose.Words24.8ช่วยเพิ่มการปรับแต่งแผนภูมิด้วยการควบคุมที่แม่นยำกว่าฉลากแกนขยายการจัดการแบบอักษรปรับปรุงการจัดการโครงสร้างเอกสารและเพิ่มความสามารถใหม่สำหรับHTML/XAMLการส่งออกPDFฟังก์ชันการแปลงเอกสารและลายเซ็นดิจิทัล.

### รูปแบบที่รองรับ

เริ่มต้นจากรุ่น24.7ส่งออกไปยังPDF/UA-2ได้รับการสนับสนุนเพื่อให้แน่ใจว่าการเข้าถึงสำหรับผู้ใช้ที่มีค.

### การแสดงผลและการพิมพ์

#### การเปลี่ยนแปลงในแผนภูมิรูปร่างและDrawingML <sup>24.5</sup>

* เอฟเฟกต์DrawingMLแสดงผลสำหรับSVGกราฟิกซึ่งขยายฟังก์ชันการทำงานก่อนหน้านี้จำกัดเฉพาะภาพ.
* การสนับสนุนสำหรับการสร้างแผนภูมิคำสั่งผสมและการปรับคุณสมบัติเช่นความกว้างช่องว่างทับซ้อนและสเกลฟองภายในกลุ่มซีรีส์ได้รับการแนะนำโดยการเพิ่มชั้นเรียน[ChartSeriesGroup](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroup/)และ[ChartSeriesGroupCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseriesgroupcollection/)และคุณสมบัติ[series_groups](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chart/series_groups/).
* ฟังก์ชันการทำงานในการจัดการผลSoftEdgeของรูปร่างได้รับการดำเนินการโดยการเพิ่ม[SoftEdgeFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing/softedgeformat/)คลาส.
* ความสามารถในการปรับเปลี่ยนค่าของรูปร่างได้รับการดำเนินการโดยการเพิ่ม**AdjustmentCollection**และ**Adjustment**ชั้นเรียนสาธารณะและคุณสมบัติ[adjustments](https://reference.aspose.com/words/python-net/aspose.words.drawing/shape/adjustments/).

#### การเปลี่ยนแปลงในแผนภูมิรูปร่างและรูปวาด <sup>24.6</sup>

- ความสามารถในการสร้างแผนภูมิได้รับการปรับปรุง ตอนนี้คุณสามารถสร้างความหลากหลายของแผนภูมิที่กว้างขึ้นรวมถึง*Treemaps*, *Sunbursts*, *Histograms*, *Pareto* แผนภูมิ*Box & Whisker*แผนภูมิ*Waterfalls*และ*Funnels* ยให้คุณเห็นภาพข้อมูลของคุณในทางที่หลากหลายมากขึ้นและให้ข้อมูล.
- การควบคุมสีสำหรับการจัดรูปแบบเงาได้รับการปรับปรุง คุณสามารถควบคุมรูปลักษณ์ของเอกสารของคุณได้อย่างแม่นยำยิ่งขึ้นโดยการเข้าถึงสีเงา.
- เพิ่มประสิทธิภาพการทำงานสำหรับการแสดงผลพื้นหลังได้รับการปรับปรุง คุณอย่างมีนัยสำคัญสามารถเพิ่มความเร็วในการแสดงผลของภูมิหลังที่มีองค์ประกอบขนาด.
- การไล่ระดับสีที่สมจริงสำหรับรูปร่างได้รับการเพิ่ม ตอนนี้คุณสามารถสร้างDMLรูปทรงที่มีการไล่ระดับสีที่ไม่ใช่เชิงเส้น,เลียนแบบสไตล์ภาพของMicrosoft Wordเพื่อ.

#### การปรับแต่งฉลากข้อมูลแผนภูมิ <sup>24.7</sup>

ความสามารถในการปรับแต่งป้ายข้อมูลแผนภูมิเช่น**Orientation**และ**Rotation**ได้ถูกเพิ่ม.

#### จัดแต่งทรงผมจำนวนที่กำหนดเองสำหรับระดับรายการ <sup>24.7</sup>

มีการเพิ่มตัวตั้งค่าสำหรับคุณสมบัติสาธารณะ[custom_number_style_format](https://reference.aspose.com/words/python-net/aspose.words.lists/listlevel/custom_number_style_format/) ตอนนี้คุณสามารถกำหนดจัดแต่งทรงผมจำนวนที่กำหนดเองสำหรับระดับรายการ.

#### การเปลี่ยนแปลงในการทำงานกับActiveX <sup>24.7</sup>

- คุณสมบัติของActiveXออบเจกต์สามารถถูกแก้ไขได้ในขณะนี้ซึ่งจะช่วยให้คุณสามารถควบคุมพฤติกร.
- ความสามารถในการปรับเปลี่ยนค่าของปุ่มควบคุมActiveXเพื่อเปิดใช้งานการโต้ตอบแบบไดนามิก.
- ความสามารถในการสลับActiveXcheckboxเป็น"ถูกเลือก"หรือ"ไม่ถูกเลือก"ถูกเพิ่ม.

#### ควบคุมแกนแผนภูมิป้ายติ๊กป้ายการวางแนวทางและการหมุน <sup>24.8</sup>

การควบคุมการวางแนวและการหมุนของฉลากติ๊กแกนแผนภูมิที่แม่นยำสำหรับการปรับแต่งแผนภูมิที่สะดวกยิ่งขึ้น-ชั้น[AxisTickLabels](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/)ได้รับการขยายด้วยคุณสมบัติใหม่[orientation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/orientation/)และ[rotation](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/axisticklabels/rotation/).

#### การเปลี่ยนเครื่องหมายทับด้วยป้ายเงินเยน <sup>24.8</sup>

ย้อนกลับเข้ากันได้HTMLและXAMLการส่งออกสำหรับการแทนที่อักขระเครื่องหมายเงินเยนได้รับการ เพื่อให้บรรลุนี้คุณสมบัติ**replace_backslash_with_yen_sign**ได้ถูกเพิ่มเข้าไปในชั้นเรียน[HtmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/htmlsaveoptions/)และ[XamlFlowSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xamlflowsaveoptions/).

#### การใช้แท็กSDTเป็นชื่อฟิลด์ฟอร์มเมื่อส่งออกไปยังPDF <sup>24.8</sup>

การส่งออก PDF พร้อมรองรับการใช้แท็ก SDT เป็นชื่อฟิลด์ฟอร์มได้รับการปรับปรุงโดยการเพิ่มคุณสมบัติ [use_sdt_tag_as_form_field_name](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/use_sdt_tag_as_form_field_name/) ใหม่ลงในคลาส [PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/).

### การแปลงโหลดและบันทึกเอกสาร

#### กำลังส่งออกลิงก์ไปยังรูปแบบMarkdown <sup>24.7</sup>

ความสามารถในการควบคุมการส่งออกลิงก์ในรูปแบบMarkdownได้ถูกเพิ่มผ่านการนำคุณสมบัติ[link_export_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/link_export_mode/)ไปใช้.

#### LowCode 24.8 <sup>24.8</sup>

คลาสใหม่[LowCode.Converter](https://reference.aspose.com/words/python-net/aspose.words.lowcode/converter/)ออกแบบมาเพื่อให้ชุดของวิธีการสำหรับการแปลงชนิดเอกสารต่างๆที่มีบรรทัดเดี.

### ค้นหาและเปรียบเทียบ

#### ตัวเลือกการเปรียบเทียบขั้นสูง <sup>24.6</sup>

ความสามารถในการปรับปรุงเวิร์กโฟลว์การวิเคราะห์ข้อมูลที่มีฟังก์ชั่นการเปรียบเทียบที่ อ็อพชัน[ignore_store_item_id](https://reference.aspose.com/words/python-net/aspose.words.comparing/advancedcompareoptions/ignore_store_item_id/)ใหม่และอินเทอร์เฟซที่ออกแบบใหม่สำหรับการเปรียบเทียบขั้นสูง.

### อื่นๆ

* ฟังก์ชันในการกำจัดหน้าว่างออกจากเอกสารได้ถูกนำมาใช้โดยการเพิ่มวิธีการ[remove_blank_pages](https://reference.aspose.com/words/python-net/aspose.words/document/remove_blank_pages/) <sup>24.5</sup>
* ความสามารถในการตรวจสอบสถานะของแมโครVBAโดยไม่ต้องโหลดเอกสารได้โดยการเพิ่มคุณสมบัติ[has_macros](https://reference.aspose.com/words/python-net/aspose.words/fileformatinfo/has_macros/) <sup>24.5</sup>
* การเก็บหมายเลขแหล่งที่มาในขณะที่แทรกเอกสารโดยใช้เครื่องมือการรายงานLINQได้รับการสนับสนุนในขณะนี้ <sup>24.5</sup>
* มีการเพิ่มคุณสมบัติใหม่[date_time_utc](https://reference.aspose.com/words/python-net/aspose.words/comment/date_time_utc/)ซึ่งจะช่วยให้การประทับเวลาที่แม่นยำยิ่งขึ้นสำหรับความคิดเห็นปรับปรุงองค์กรและการตรวจสอบย้อนกลับ <sup>24.6</sup>
* รูปแบบวันที่จะถูกตรวจพบโดยอัตโนมัติสำหรับการส่งออกที่ไร้รอยต่อไปยังรูปแบบXLSX <sup>24.7</sup>
* คุณสมบัติสาธารณะ[is_protected](https://reference.aspose.com/words/python-net/aspose.words.vba/vbaproject/is_protected/)ซึ่งช่วยให้คุณสามารถตรวจสอบว่าโครงการVBAได้รับการป้องกัน,มีการเ <sup>24.7</sup>
* ข้อมูลแบบอักษรถูกขยายด้วยคุณสมบัติของ**embedding_licensing_rights**ที่เพิ่มเข้าไปในชั้นเรียน[FontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/fontinfo/)และ[PhysicalFontInfo](https://reference.aspose.com/words/python-net/aspose.words.fonts/physicalfontinfo/) <sup>24.8</sup>
* วิธีการล้างส่วนหัวและท้ายกระดาษได้อย่างมีประสิทธิภาพในขณะที่เก็บรักษาลายน้ำได้ถูก เมื่อต้องการล้างส่วนหัวและท้ายกระดาษให้ใช้วิธีการสาธารณะใหม่[clear_headers_footers](https://reference.aspose.com/words/python-net/aspose.words/section/clear_headers_footers/#default) <sup>24.8</sup>
* การลงลายเซ็นดิจิทัลของXPSเอกสารที่ใช้[XpsSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/)ได้ถูกเปิดใช้งานแล้ว-มีการเพิ่มคุณสมบัติใหม่[digital_signature_details](https://reference.aspose.com/words/python-net/aspose.words.saving/xpssaveoptions/digital_signature_details/)เพื่อจุดประสงค์นี้ <sup>24.8</sup>

{{% alert color="primary" %}}

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 24.5บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-5-release-notes/).

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 24.6บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-6-release-notes/).

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 24.7บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-7-release-notes/).

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 24.8บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-8-release-notes/).

{{% /alert %}}

## Aspose.Words สำหรับ Python ผ่านทาง .NET 24.1, 24.2, 24.3, 24.4

Aspose.Words24.1ปรับปรุงประสบการณ์การจัดการสีจังหวะช่วยเพิ่มOLEวัตถุ,เช่นเดียวกับการแนะนำใหม่`Bibliography Sources`สาธารณะAPI.

Aspose.Words24.2แผนภูมิขยายAPIและการจัดการสไตล์. รุ่นของAspose.Wordsนี้ยังแนะนำความสามารถในการระบุSvgSaveOptionsในระหว่างการแสดงผล,การควบคุมที่ยืดหยุ่นมากขึ้นในการโหลดMarkdownไฟล์,และการทำงานกับข้อความอ้างอิงสำหรับเชิงอรรถและหมายเหตุสิ้นสุด.

Aspose.Words24.3แนะนำใหม่TIFFผู้อ่าน/นักเขียนและการจำลองการดำเนินงานแรสเตอร์ไบนารีสำหรับWMFเมต Aspose.Words24.3ยังคงขยายแผนภูมิAPI.

Aspose.Words24.4ปรับปรุงรูปแบบการบันทึก,ตัวเลือกการแสดงผลบางอย่าง,เช่นเดียวกับการปรับปรุงการท.

### รูปแบบที่รองรับ <sup>24.4</sup>

รูปแบบภาพที่ทันสมัย**WebP**ได้รับการสนับสนุนในขณะนี้ใน Aspose.Wordsสำหรับ.NET Framework 4.6.2 และสูงกว่า ขณะนี้คุณสามารถอ่านและแทรกภาพWebPลงในเอกสารรวมทั้งบันทึกภาพในรูปแบบWebP.

โปรดทราบว่าWebPปัจจุบันมีให้บริการเฉพาะใน.NET Standardและ.NET Frameworkวี4.6.2ขึ้นไป.

### การแสดงผลและการพิมพ์

#### การควบคุมสีจังหวะ <sup>24.1</sup>

ชั้น[Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/)ได้รับการขยายด้วยชุดของคุณสมบัติสาธารณะใหม่ที่เกี่ยวข้องกับการจัดการสีจังหวะ:[fore_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_theme_color/)และ[back_theme_color](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_theme_color/),[fore_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/fore_tint_and_shade/)และ[back_tint_and_shade](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/back_tint_and_shade/).

#### DrawingMLแผนภูมิAPIส่วนขยาย <sup>24.2 / 24.3 / 24.4</sup>

ขยาย**DrawingML Charts API**ต่อไป.

#### ฝังแบบอักษรที่ประกาศในกฎ@font-face <sup>24.4</sup>

เพิ่มความสามารถในการฝังแบบอักษรที่ประกาศในกฎ@font-faceลงในคำจำกัดความแบบอักษรของเอกสารที่ได้ถูกนำมาใช้โดยการเพิ่มคุณสมบัติใหม่[support_font_face_rules](https://reference.aspose.com/words/python-net/aspose.words.loading/htmlloadoptions/support_font_face_rules/).

#### ทำงานร่วมกับเรืองแสงและการสะท้อนรูปแบบ <sup>24.4</sup>

ความสามารถในการทำงานร่วมกับการเรืองแสงและการสะท้อนการจัดรูปแบบสำหรับวั.

### การโหลดและบันทึกเอกสาร

#### ระบุSvgSaveOptionsระหว่างการแสดงผล <sup>24.2</sup>

ความสามารถในการระบุ[SvgSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/svgsaveoptions/)ระหว่างการแสดงผลถูกเพิ่มโดยใช้[ShapeRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/shaperenderer/)[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions)และ[OfficeMathRenderer](https://reference.aspose.com/words/python-net/aspose.words.rendering/officemathrenderer/)[save](https://reference.aspose.com/words/python-net/aspose.words.rendering/noderendererbase/save/#bytesio_svgsaveoptions)วิธีการ.

#### เก็บบรรทัดว่างไว้เมื่อโหลดไฟล์Markdown <sup>24.2</sup>

ความสามารถในการรักษาบรรทัดว่างเมื่อโหลดMarkdownไฟล์ถูกเพิ่ม.

#### ใหม่TIFFผู้อ่าน/นักเขียน <sup>24.3</sup>

มีการพัฒนาโปรแกรมอ่าน/นักเขียนใหม่TIFFสำหรับAspose.Words Aspose.Wordsสำหรับ.NET 24.3 เพิ่มการสนับสนุนสำหรับการอ่านTIFFภาพที่มีJPEGและเก่าJPEGชนิดการบีบอัดและยังปรับปรุงคุณภาพ.

### อื่นๆ

* ความสามารถในการปรับเปลี่ยนข้อความของ`TextBox`OLEตัวควบคุมได้รับการแนะนำโดยการเพิ่มคุณสมบัติ**Text**ใหม่ไปยังคลาสใหม่**TextBoxControl** <sup>24.1</sup>
* แหล่งบรรณานุกรมสาธารณะAPIถูกนำมาใช้ผ่านการเพิ่มเนมสเปซใหม่[Aspose.Words.Bibliography](https://reference.aspose.com/words/python-net/aspose.words.bibliography/)กับชั้นเรียนใหม่และการแจงนับและผ่านการเพิ่มคุณสมบัติใหม่[bibliography](https://reference.aspose.com/words/python-net/aspose.words/document/bibliography/)ลงในชั้นเรียน[Document](https://reference.aspose.com/words/python-net/aspose.words/document/) <sup>24.1</sup>
* คุณสมบัติสาธารณะใหม่[priority](https://reference.aspose.com/words/python-net/aspose.words/style/priority/),[unhide_when_used](https://reference.aspose.com/words/python-net/aspose.words/style/unhide_when_used/)และ[semi_hidden](https://reference.aspose.com/words/python-net/aspose.words/style/semi_hidden/)สำหรับการจัดการสไตล์ที่เพิ่มขึ้นได้รับการเพิ่มในชั้นเรียน[Style](https://reference.aspose.com/words/python-net/aspose.words/style/) <sup>24.2</sup>
* งหมายอ้างอิงจริงสำหรับเชิงอรรถและหมายเหตุสิ้นสุดได้รับการปรับปรุงด้วยคุณสมบัติ[actual_reference_mark](https://reference.aspose.com/words/python-net/aspose.words.notes/footnote/actual_reference_mark/)และ[update_actual_reference_marks](https://reference.aspose.com/words/python-net/aspose.words/document/update_actual_reference_marks/#default) <sup>24.2</sup>
* มีการดำเนินการจำลองการดำเนินงานแรสเตอร์ไบนารีสำหรับWMFเมตาไฟล์ <sup>24.3</sup>
* ความสามารถในการกำหนดตัวเลือกลายเซ็นสำหรับเอกสารภายใน**SaveOptions**ถูกเปิดใช้งานโดยการเพิ่มคลาสใหม่[DigitalSignatureDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/digitalsignaturedetails/)กับสมาชิกสาธารณะใหม่รวมทั้งการเพิ่มคุณสมบัติใหม่ในคลาส[OoxmlSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/ooxmlsaveoptions/),[DocSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/docsaveoptions/)และ[OdtSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/odtsaveoptions/) <sup>24.4</sup>

{{% alert color="primary" %}}

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 24.1บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-1-release-notes/).

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 24.2บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-2-release-notes/).

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 24.3บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-3-release-notes/).

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 24.4บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2024/aspose-words-for-python-via-dotnet-24-4-release-notes/).

{{% /alert %}}

## Aspose.Words สำหรับ Python ผ่านทาง .NET 23.9, 23.10, 23.11, 23.12

Aspose.Words23.9ขยายตัวเลือกการแสดงผล,การจำลองการแสดงผลเมตาไฟล์,และmarkdownบันทึกตัวเลือก.

Aspose.Words23.10ปรับปรุงการแสดงผล,ขยายตัวเลือกสำหรับการโหลดและบันทึกเอกสาร,และช่วยให้ผู้ใช้สามารถผสานเอกสารในรูปแบบใหม่.

Aspose.Words23.11ช่วยเพิ่มการทำงานที่มีการแก้ไขXLSXรูปแบบและแบบอักษรในตำนานแผนภูมิที่มีตัวเลือกเพิ่ม.

Aspose.Words23.12แนะนำคุณสมบัติใหม่และการแจงนับสำหรับการทำงานกับPDFและOOXMLเอกสารเช่นเดียวกับการสนับสนุนสำหรับWebPภาพ.

### การแสดงผลและการพิมพ์

#### การปรับแต่งชื่อแกนในDrawingMLแผนภูมิ <sup>23.9</sup>

ความสามารถในการปรับแต่งชื่อแกนในDrawingMLแผนภูมิได้ถูกนำมาใช้โดยการใช้คุณสมบัติสาธารณะใหม่[ChartAxisTitle](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxistitle/)และ[title](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartaxis/title/).

####  การกำหนดตำแหน่งแนวตั้งของแบบอักษรภายในย่อหน้า <sup>23.9</sup>

ขณะนี้สามารถกำหนดตำแหน่งแนวตั้งของแบบอักษรภายในย่อหน้าโดยใช้คุณสมบัติสาธารณะ[baseline_alignment](https://reference.aspose.com/words/python-net/aspose.words/paragraphformat/baseline_alignment/)ใหม่และการแจงนับใหม่[BaselineAlignment](https://reference.aspose.com/words/python-net/aspose.words/baselinealignment/).

#### การควบคุมสีพื้นหน้า <sup>23.10</sup>

ความสามารถในการดึงสีพื้นหน้าโดยไม่มีการปรับเปลี่ยนได้ถูกเพิ่มเข้าไปในชั้นเรียน[Fill](https://reference.aspose.com/words/python-net/aspose.words.drawing/fill/)และ[Stroke](https://reference.aspose.com/words/python-net/aspose.words.drawing/stroke/)ผ่านคุณสมบัติของ**BaseForeColor**.

#### ขยายฟังก์ชันการทำงานของแผนภูมิ <sup>23.10</sup>

ฟังก์ชันการทำงานของ[ChartDataPointCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartdatapointcollection/),[ChartSeries](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartseries/)และ[ChartFormat](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartformat/)คลาสได้รับการขยายด้วยวิธีการและคุณสมบัติใหม่.

#### ปรับและพอดีกับภาพเป็นรูปร่างโดยอัตโนมัติ <sup>23.10</sup>

วิธีง่ายๆในการปรับและปรับให้พอดีกับรูปภาพภายในรูปร่างเฉพาะได้ผ่านทางวิธีใหม่[fit_image_to_shape](https://reference.aspose.com/words/python-net/aspose.words.drawing/imagedata/fit_image_to_shape/#default).

#### การจัดรูปแบบแบบอักษรปริยายสำหรับรายการตำนานแผนภูมิDrawingML <sup>23.11</sup>

ความสามารถในการระบุการจัดรูปแบบฟอนต์ดีฟอลต์สำหรับรายการตำนานของDrawingMLแผนภูมิถูกเพิ่มผ่านคุณสมบัติของ[font](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartlegend/font/) นและสอดคล้องกันมากขึ้นสำหรับองค์ประกอบแผนภูมิ,การปรับปรุงความสวยงามของเอกสา.

#### ระบุเค้าโครงหน้าเมื่อเปิดPDFในตัวอ่าน <sup>23.12</sup>

ความสามารถในการระบุเค้าโครงหน้าเว็บที่จะใช้เมื่อเปิดเอกสารในเครื่องอ่านPDFได้ถูกเพิ่มผ่านการแนะนำคุณสมบัติใหม่[page_layout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/page_layout/)ให้กับคลาสของ[PdfSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfsaveoptions/)และการแนะนำการแจงนับใหม่[PdfPageLayout](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfpagelayout/).

### การโหลดและบันทึกเอกสาร

#### การระบุชื่อโฟลเดอร์ที่จะสร้างภาพURIsในMarkdown <sup>23.9</sup>

คลาส[MarkdownSaveOptions](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/)ถูกขยายโดยรวมคุณสมบัติ[images_folder_alias](https://reference.aspose.com/words/python-net/aspose.words.saving/markdownsaveoptions/images_folder_alias/)ซึ่งอนุญาตให้ระบุชื่อของโฟลเดอร์ที่ใช้สร้างภาพURIsเขียนลงในเอกสารMarkdown.

#### ลดขนาดเอาท์พุทPDF <sup>23.10</sup>

การเพิ่มประสิทธิภาพการแสดงผลต่างๆPDFเพื่อลดขนาดเอาต์พุตเมื่อใช้การตั้งค่า[optimize_output](https://reference.aspose.com/words/python-net/aspose.words.saving/fixedpagesaveoptions/optimize_output/)ถูกนำมาใช้.

#### รู้จักการเชื่อมโยงหลายมิติเมื่อโหลดเอกสารTXT <sup>23.10</sup>

คุณลักษณะในการจดจำการเชื่อมโยงหลายมิติเมื่อโหลดเอกสารTXTถูกนำมาใช้โดยการเพิ่มคุณสมบัติ[detect_hyperlinks](https://reference.aspose.com/words/python-net/aspose.words.loading/txtloadoptions/detect_hyperlinks/)ใหม่.

### อื่นๆ

- รับWMFความกว้างของปากกาและความกว้างของปากกาเครื่องสำอางEMF เพื่อให้บรรลุนี้ทรัพย์สิน**ScaleWmfFontsToMetafileSize**ถูกแทนที่ด้วยทรัพย์สิน[emulate_rendering_to_size_on_page](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page/)และทรัพย์สิน[emulate_rendering_to_size_on_page_resolution](https://reference.aspose.com/words/python-net/aspose.words.saving/metafilerenderingoptions/emulate_rendering_to_size_on_page_resolution/)ถูกเพิ่มเข้ามา <sup>23.9</sup>
- วิธีที่ง่ายสำหรับการแทรกเอกสารหนึ่งลงในเอกสารอื่นที่ตำแหน่งเคอร์เซอร์ปัจจุบันได้ถูกนำมาใช้วิธีการ[insert_document_inline](https://reference.aspose.com/words/python-net/aspose.words/documentbuilder/insert_document_inline/#document_importformatmode_importformatoptions) <sup>23.10</sup>
- มีการเพิ่มความสามารถในการเข้าถึงและแก้ไขคุณสมบัติลักษณะผ่านการแนะนำคุณสมบัติใหม่[locked](https://reference.aspose.com/words/python-net/aspose.words/style/locked/) <sup>23.10</sup>
- พารามิเตอร์ชนิดทั่วไปถูกเพิ่มเข้าไปในวิธีการของคลาสของ[CompositeNode](https://reference.aspose.com/words/python-net/aspose.words/compositenode/) <sup>23.10</sup>
- ความสามารถในการเขียนทุกส่วนของเอกสารลงในเวิร์กชีทXLSXเดียวกันได้รับการจัดให้ผ่านประเภทการแจงนับใหม่[XlsxSectionMode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsectionmode/)และคุณสมบัติใหม่[section_mode](https://reference.aspose.com/words/python-net/aspose.words.saving/xlsxsaveoptions/section_mode/) <sup>23.11</sup>
* วิธีการควบคุมวิธีใช้ส่วนขยายรูปแบบZIP64สำหรับเอกสารOOXMLผ่านคุณสมบัติโหมดไปรษณีย์64ใหม่ของคลาสของ`OoxmlSaveOptions`และการแจงนับโหมดไปรษณีย์64ใหม่ <sup>23.12</sup>
* การสนับสนุนสำหรับWebPภาพที่ได้รับการแนะนำ โปรดทราบว่าคุณลักษณะนี้ใช้ได้เฉพาะสำหรับNetStandartและ.NET6+เวอร์ชัน <sup>23.12</sup>

{{% alert color="primary" %}}

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 23.9บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-9-release-notes/).

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 23.10บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-10-release-notes/).

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 23.11บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-11-release-notes/).

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.Wordsสำหรับ.NET 23.12 บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-12-release-notes/).

{{% /alert %}}

## Aspose.Words สำหรับ Python ผ่านทาง .NET 23.5, 23.6, 23.7, 23.8

Aspose.Words23.5ช่วยเพิ่มความสามารถในการทำงานกับข้อมูลชุดแผนภูมิและความสามารถในการทำงานกับODTเอกสารเช่นเดียวกับการปรับปรุงส่วนหัว/ท้ายกระดาษและการตัดข้อความของพวกเขา.

Aspose.Words23.6ขยายตัวเลือกการแสดงผลเพิ่มรูปแบบการส่งออกใหม่ปรับปรุงการรายงานLINQและเครื่องมือLowCode.

Aspose.Words23.7ช่วยเพิ่มความสามารถในการรายงานเพิ่มรูปแบบการส่งออกใหม่และแนะนำการเปลี่ยน.

Aspose.Words23.8ขยายความสามารถของรูปแบบต่างๆปรับปรุงการแสดงผลและเพิ่มตัวเลือกใหม่สำหรับกา

### รูปแบบที่รองรับ

* เริ่มต้นด้วยเวอร์ชัน23.6คุณสามารถบันทึกเอกสารในรูปแบบXLSX ตอนนี้คุณสามารถแปลงเอกสารของคุณให้เป็นรูปแบบเก่ง <sup>23.6</sup>

* เริ่มต้นด้วยเวอร์ชัน23.7คุณสามารถบันทึกหน้าเอกสารหรือรูปร่างในรูปแบบEPS <sup>23.7</sup>

### คุณลักษณะรูปแบบใหม่

- ฟังก์ชันการทำงานที่สร้างสารบัญโดยอัตโนมัติ(TOC)สำหรับMOBIเอกสารได้รับการแนะนำ <sup>23.8</sup>
- ตัวสร้าง[PdfEncryptionDetails](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions)ถูกขยายด้วย[PdfPermissions](https://reference.aspose.com/words/python-net/aspose.words.saving/pdfencryptiondetails/__init__/#str_str_pdfpermissions) <sup>23.8</sup>
- มีการสร้างข้อความแนวตั้งสำหรับEMFเมตาไฟล์แล้ว <sup>23.8</sup>

### การแสดงผล

#### รับและปรับเปลี่ยนข้อมูลชุดแผนภูมิ <sup>23.5</sup>

คุณลักษณะที่จะได้รับและปรับเปลี่ยนข้อมูลชุดแผนภูมิที่มีให้โดยการเพิ่ม:

- คลาสใหม่: [ChartXValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvalue/), [ChartYValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvalue/), [ChartXValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluecollection/), [ChartYValueCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluecollection/), [BubbleSizeCollection](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/bubblesizecollection/), [ChartMultilevelValue](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartmultilevelvalue/)
- ประเภทเอนัมใหม่:[ChartXValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartxvaluetype/),[ChartYValueType](https://reference.aspose.com/words/python-net/aspose.words.drawing.charts/chartyvaluetype/)

#### การสนับสนุนสำหรับการพิมพ์ขั้นสูง <sup>23.6</sup>

การสนับสนุนสำหรับการพิมพ์ขั้นสูงในWMF,EMFและEMF+การแสดงผลได้รับการเพิ่ม.

#### เนื้อหาสีบนหน้าเว็บ <sup>23.6</sup>

คุณสมบัติสาธารณะ[PageInfo.colored](https://reference.aspose.com/words/python-net/aspose.words.rendering/pageinfo/colored/)ซึ่งบ่งชี้ว่าเพจเป็นสีหรือไม่มีการเพิ่มเพจ.

#### การจัดรูปแบบสำหรับป้ายกำกับข้อมูลแผนภูมิ <sup>23.6</sup>

ความสามารถในการตั้งค่าการเติม,จังหวะ,และการจัดรูปแบบคำบรรยายภาพสำหรับฉลากข้.

### Mail Mergeและการรายงาน

#### แทรกแบบไดนามิกHTMLสำหรับLINQเครื่องมือการรายงาน <sup>23.6</sup>

มีการเพิ่มวิธีการใหม่ของการแทรกแบบไดนามิกHTMLสำหรับLINQเครื่องมือการรายงาน.

#### Mustacheแท็กสนับสนุน <sup>23.7</sup>

ขณะนี้รองรับแท็กMustacheในวิธีการ[MailMerge.GetRegionsHierarchy](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_regions_hierarchy/)และ[MailMerge.GetFieldNamesForRegion](https://reference.aspose.com/words/python-net/aspose.words.mailmerging/mailmerge/get_field_names_for_region/).

#### การระบุขนาดของภาพที่แสดงผล <sup>23.8</sup>

มีการแนะนำคุณสมบัติสาธารณะใหม่[image_size](https://reference.aspose.com/words/python-net/aspose.words.saving/imagesaveoptions/image_size/)สำหรับการระบุขนาดของภาพที่แสดงผลเป็นพิกเซล.

#### รักษาช่องว่างสำหรับค่าสตริงJSON–LINQ <sup>23.8</sup>

มีการเพิ่มตัวเลือกลงในโปรแกรมการรายงานLINQเพื่อรักษาช่องว่างสำหรับค่าสตริงJSON.

### LowCode <sup>23.6</sup>

มีการเพิ่มวิธีการใหม่LowCodeเพื่อผสานเอกสารประเภทต่างๆลงในเอกสารที่ส่งออกเดียว.

### อื่นๆ

- การสนับสนุนสำหรับการตัดข้อความในส่วนหัว/ส่วนท้ายได้รับการดำเนินการ <sup>23.5</sup>
- ความสามารถในการลบลายเซ็นดิจิทัลออกจากเอกสารODTได้ถูกเพิ่มผ่านวิธีการ[RemoveAllSignatures](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignatureutil/remove_all_signatures/#str_str) <sup>23.5</sup>
- ทรัพย์สินสาธารณะ[phonetic_guide](https://reference.aspose.com/words/python-net/aspose.words/run/phonetic_guide/)ที่จะได้รับข้อความฐานและทับทิมของคู่มือการออกเสียง[Run](https://reference.aspose.com/words/python-net/aspose.words/run/)ได้รับการเพิ่ม <sup>23.5</sup>
- ความสามารถในการดึงค่าลายเซ็นดิจิทัลจากเอกสารที่ลงนามแบบดิจิทัลเป็นอาร์เรย์ไบต์ถูกเพิ่มโดยการแนะนำคุณสมบัติใหม่[signature_value](https://reference.aspose.com/words/python-net/aspose.words.digitalsignatures/digitalsignature/signature_value/) <sup>23.7</sup>
- ชั้นเรียน[Row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/)และ[Cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/)ได้รับการขยายไปพร้อมกับสมาชิกสาธารณะใหม่– [Row.next_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/next_row/), [Row.previous_row](https://reference.aspose.com/words/python-net/aspose.words.tables/row/previous_row/), [Cell.next_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/next_cell/), และ[Cell.previous_cell](https://reference.aspose.com/words/python-net/aspose.words.tables/cell/previous_cell/) <sup>23.7</sup>

{{% alert color="primary" %}}

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 23.5บันทึกย่อ](/words/python-net/aspose-words-for-python-via-dotnet-23-5-release-notes/).

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 23.6บันทึกย่อ](/words/python-net/aspose-words-for-python-via-dotnet-23-6-release-notes/).

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 23.7บันทึกย่อ](https://releases.aspose.com/words/python/release-notes/2023/aspose-words-for-python-via-dotnet-23-7-release-notes/).

เรียนรู้เพิ่มเติมเกี่ยวกับ [Aspose.WordsสำหรับPython via .NET 23.8บันทึกย่อ](/words/python-net/aspose-words-for-python-via-dotnet-23-8-release-notes/).

{{% /alert %}}

## ดูเพิ่มเติม

{{% alert color="primary" %}}

หน้านี้ประกอบด้วยข่าวล่าสุดสำหรับที่ผ่านมา 2 ปี สำหรับรายละเอียดเกี่ยวกับรุ่นก่อนหน้านี้ให้ดูที่ [บันทึกย่อ'](https://releases.aspose.com/words/python/release-notes/) หน้าในส่วนที่เกี่ยวข้อง.

{{% /alert %}}
