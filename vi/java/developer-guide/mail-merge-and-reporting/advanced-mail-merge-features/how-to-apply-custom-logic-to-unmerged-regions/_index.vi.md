---
title: Cách Áp dụng Logic Tùy chỉnh Cho Các Khu Vực Chưa Được Hợp Nhất
second_title: Aspose.Words cho Java
articleTitle: Cách Áp dụng Logic Tùy chỉnh Cho Các Khu Vực Chưa Được Hợp Nhất
linktitle: Cách Áp dụng Logic Tùy chỉnh Cho Các Khu Vực Chưa Được Hợp Nhất
type: docs
description: "Áp dụng logic tùy chỉnh cho các vùng chưa được hợp nhất trong thao tác Mail Merge bằng Java."
weight: 70
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /vi/java/how-to-apply-custom-logic-to-unmerged-regions/
timestamp: 2024-01-27-14-07-04
---

Có một số trường hợp không mong muốn xóa hoàn toàn các vùng chưa hợp nhất khỏi tài liệu trong Mail Merge hoặc dẫn đến tài liệu trông không đầy đủ. Điều này có thể xảy ra khi không có dữ liệu đầu vào sẽ được hiển thị cho người dùng dưới dạng tin nhắn thay vì khu vực bị xóa hoàn toàn.

Cũng có những lúc việc tự mình xóa vùng không sử dụng là không đủ, ví dụ, nếu vùng có trước tiêu đề hoặc vùng được chứa trong bảng. Nếu vùng này không được sử dụng thì tiêu đề và bảng sẽ vẫn còn sau khi vùng bị xóa sẽ trông không đúng vị trí trong tài liệu.

Bài viết này cung cấp một giải pháp để xác định thủ công cách xử lý các vùng không sử dụng trong tài liệu. Mã cơ sở cho chức năng này được cung cấp và có thể dễ dàng sử dụng lại trong một dự án khác.

Logic được áp dụng cho mỗi vùng được xác định bên trong một lớp thực hiện giao diện [IFieldMergingCallback](https://reference.aspose.com/words/java/com.aspose.words/ifieldmergingcallback/). Theo cách tương tự, trình xử lý Mail Merge có thể được thiết lập để kiểm soát cách từng trường được hợp nhất, trình xử lý này có thể được thiết lập để thực hiện các hành động trên từng trường trong một khu vực không sử dụng hoặc trên toàn bộ khu vực. Trong trình xử lý này, bạn có thể đặt mã để thay đổi văn bản của một khu vực, xóa các nút hoặc các hàng và ô trống, v. v.

Trong mẫu này, chúng tôi sẽ sử dụng tài liệu được hiển thị bên dưới. Nó chứa các vùng lồng nhau và một vùng chứa trong bảng.

![apply-custom-logic-to-unmerged-regions-aspose-words-java](how-to-apply-custom-logic-to-unmerged-regions-1.png)

Để trình diễn nhanh, chúng ta có thể thực thi cơ sở dữ liệu mẫu trên tài liệu mẫu với cờ [MailMergeCleanupOptions.REMOVE_UNUSED_REGIONS](https://reference.aspose.com/words/java/com.aspose.words/mailmergecleanupoptions/) được bật. Thuộc tính này sẽ tự động xóa các vùng chưa được hợp nhất khỏi tài liệu trong mail merge.

Nguồn dữ liệu bao gồm hai bản ghi cho vùng **StoreDetails** nhưng có mục đích có bất kỳ dữ liệu nào cho vùng **ContactDetails** con cho một trong các bản ghi. Hơn nữa, vùng **Suppliers** cũng không có bất kỳ hàng dữ liệu nào. Điều này sẽ khiến các khu vực không sử dụng vẫn còn trong tài liệu. Kết quả sau khi hợp nhất tài liệu với nguồn dữ liệu này là dưới đây.

![merged-regions-aspose-words-java](how-to-apply-custom-logic-to-unmerged-regions-2.png)

Như đã lưu ý trên hình ảnh, bạn có thể thấy rằng vùng **ContactDetails** cho bản ghi thứ hai và vùng **Suppliers** đã tự động bị xóa bởi công cụ Mail Merge vì chúng không có dữ liệu. Tuy nhiên, có một số vấn đề khiến tài liệu đầu ra này trông không đầy đủ:

- Vùng **ContactDetails** vẫn để lại một đoạn văn có dòng chữ "Chi tiết Liên hệ".
- Trong trường hợp tương tự, không có dấu hiệu cho thấy không có số điện thoại, chỉ có một khoảng trống có thể dẫn đến nhầm lẫn.
- Bảng và tiêu đề liên quan đến vùng **Suppliers** cũng vẫn còn sau khi vùng bên trong bảng bị xóa.

Kỹ thuật được cung cấp trong bài viết này thể hiện cách áp dụng logic tùy chỉnh cho từng khu vực chưa được hợp nhất để tránh những vấn đề này.

**Giải Pháp**

Để áp dụng logic theo cách thủ công cho từng khu vực không sử dụng trong tài liệu, chúng tôi tận dụng các tính năng đã có sẵn trong Aspose.Words.

Động cơ Mail Merge cung cấp một thuộc tính để loại bỏ các vùng không sử dụng thông qua cờ **MailMergeCleanupOptions.RemoveUnusedRegions**. Điều này có thể bị vô hiệu hóa để các khu vực như vậy không bị ảnh hưởng trong mail merge. Điều này cho phép chúng tôi rời khỏi các khu vực chưa được hợp nhất trong tài liệu và tự xử lý chúng theo cách thủ công.

Sau đó, chúng ta có thể tận dụng thuộc tính **MailMerge.FieldMergingCallback** như một phương tiện để áp dụng logic tùy chỉnh của riêng mình cho các vùng chưa được hợp nhất này trong Mail Merge thông qua việc sử dụng lớp xử lý triển khai giao diện **IFieldMergingCallback**.

Mã này trong lớp handler là lớp duy nhất bạn sẽ cần sửa đổi để kiểm soát logic được áp dụng cho các vùng chưa được hợp nhất. Mã khác trong mẫu này có thể được sử dụng lại mà không cần sửa đổi trong bất kỳ dự án nào.

Dự án mẫu này thể hiện kỹ thuật này. Nó bao gồm các bước sau:

1. Thực thi Mail Merge trên tài liệu bằng nguồn dữ liệu của bạn. Cờ **MailMergeCleanupOptions.RemoveUnusedRegions** bị vô hiệu hóa bây giờ chúng tôi muốn các khu vực vẫn còn để chúng tôi có thể xử lý chúng theo cách thủ công. Bất kỳ khu vực nào không có dữ liệu sẽ không được hợp nhất trong tài liệu.
1. Gọi phương thức **ExecuteCustomLogicOnEmptyRegions**. Phương pháp này được cung cấp trong mẫu này. Nó thực hiện các hành động cho phép trình xử lý được chỉ định được gọi cho từng khu vực chưa được hợp nhất. Phương pháp này có thể tái sử dụng và có thể được sao chép không thay đổi cho bất kỳ dự án nào yêu cầu nó (cùng với bất kỳ phương thức phụ thuộc nào).Phương pháp này thực hiện các bước sau:
   1. Đặt trình xử lý do người dùng chỉ định thành thuộc tính **MailMerge.FieldMergingCallback**.
   1. Gọi phương thức **CreateDataSourceFromDocumentRegions** chấp nhận **Document** và **ArrayList** của người dùng chứa tên vùng. Phương pháp này sẽ tạo một nguồn dữ liệu giả chứa các bảng cho từng vùng chưa được hợp nhất trong tài liệu.
   1. Thực thi Mail Merge trên tài liệu bằng nguồn dữ liệu giả. Khi Mail Merge được thực thi với nguồn dữ liệu này, nó cho phép trình xử lý do người dùng chỉ định được gọi cho từng vùng chưa hợp nhất và logic tùy chỉnh được áp dụng

**Mã**

Việc triển khai phương thức **ExecuteCustomLogicOnEmptyRegions** được tìm thấy bên dưới. Phương pháp này chấp nhận một số tham số:

1. Đối tượng [Document](https://reference.aspose.com/words/java/com.aspose.words/document/) chứa các vùng chưa được hợp nhất sẽ được xử lý bởi trình xử lý được thông qua.
1. Lớp xử lý xác định logic để áp dụng cho các vùng chưa được hợp nhất. Trình xử lý này phải thực hiện [IFieldMergingCallback](https://www.aspose.com/api/java/words/com.aspose.words/interfaces/IFieldMergingCallback) giao diện.
1. Thông qua việc sử dụng quá tải thích hợp, phương thức cũng có thể chấp nhận tham số thứ ba – danh sách tên vùng dưới dạng chuỗi. Nếu điều này được chỉ định thì chỉ các tên khu vực còn lại tài liệu được chỉ định trong danh sách sẽ được xử lý thủ công. Các khu vực khác gặp phải sẽ không được trình xử lý gọi và tự động xóa. Khi quá tải chỉ với hai tham số được chỉ định, mọi khu vực còn lại trong tài liệu được bao gồm bởi phương thức được xử lý thủ công.

**Ví dụ**

Hiển thị cách thực thi logic tùy chỉnh trên các vùng không sử dụng bằng trình xử lý được chỉ định.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-ExecuteCustomLogicOnUnusedRegions.java" >}}

{{% alert color="primary" %}}

Nếu bạn xem xét chạy phương thức **ExecuteCustomLogicOnEmptyRegions** liên tiếp với các trình xử lý khác nhau (ví dụ: mỗi trình xử lý áp dụng logic cho các trường nhất định) thì bạn sẽ cần vô hiệu hóa việc xóa các vùng không sử dụng để các vùng đó không bị xóa giữa các cuộc gọi này.

{{% /alert %}}

**Ví dụ**

Xác định phương pháp được sử dụng để xử lý thủ công các vùng chưa được hợp nhất.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-ManuallyHandleUnmergedRegions.java" >}}

Phương pháp này liên quan đến việc tìm kiếm tất cả các khu vực chưa được hợp nhất trong tài liệu. Điều này được thực hiện bằng phương pháp **MailMerge.GetFieldNames**. Phương thức này trả về tất cả các trường hợp nhất trong tài liệu, bao gồm các điểm đánh dấu bắt đầu và kết thúc khu vực (được biểu thị bằng các trường hợp nhất với tiền tố *TableStart* hoặc *TableEnd*).

Khi gặp trường hợp nhất `TableStart`, trường này được thêm dưới dạng mới **DataTable** vào **DataSet**. Vì một vùng có thể xuất hiện nhiều lần (ví dụ vì nó là một vùng lồng nhau trong đó vùng cha đã được hợp nhất với nhiều bản ghi), bảng chỉ được tạo và thêm nếu nó chưa tồn tại trong **DataSet**.

Khi một vùng bắt đầu thích hợp đã được tìm thấy và thêm vào cơ sở dữ liệu, trường tiếp theo (tương ứng với trường đầu tiên trong vùng) được thêm vào **DataTable**. Chỉ cần thêm trường đầu tiên cho mỗi trường trong khu vực để được hợp nhất và chuyển cho trình xử lý.

Chúng tôi cũng đặt giá trị trường của trường đầu tiên thành "FirstField" để dễ dàng áp dụng logic cho các trường đầu tiên hoặc các trường khác trong khu vực. Bằng cách bao gồm điều này, điều đó có nghĩa là không cần thiết phải mã hóa cứng tên của trường đầu tiên hoặc thực hiện mã bổ sung để kiểm tra xem trường hiện tại có phải là trường đầu tiên trong mã xử lý hay không.

Đoạn mã dưới đây cho thấy hệ thống này hoạt động như thế nào. Tài liệu được hiển thị ở đầu bài viết này được phối lại với cùng một nguồn dữ liệu nhưng lần này, các vùng không sử dụng được xử lý bằng mã tùy chỉnh.

**Ví dụ**

Hiển thị cách xử lý các vùng chưa được hợp nhất sau Mail Merge với mã do người dùng xác định.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-HandleUnmergedRegionsAfterMailMerge.java" >}}


Mã thực hiện các thao tác khác nhau dựa trên tên của khu vực được truy xuất bằng thuộc tính **FieldMergingArgs.TableName**. Lưu ý rằng tùy thuộc vào tài liệu và khu vực của bạn, bạn có thể mã hóa trình xử lý để chạy logic phụ thuộc vào từng khu vực hoặc mã áp dụng cho mọi khu vực chưa được hợp nhất trong tài liệu hoặc kết hợp cả hai.

Logic cho vùng **ContactDetails** liên quan đến việc thay đổi văn bản của từng trường trong vùng **ContactDetails** với một thông báo thích hợp cho biết rằng không có dữ liệu. Tên của mỗi trường được khớp trong trình xử lý bằng thuộc tính **FieldMergingArgs.FieldName**.

Một quy trình tương tự được áp dụng cho vùng **Suppliers** với việc bổ sung thêm mã để xử lý bảng chứa vùng. Mã sẽ kiểm tra xem khu vực có được chứa trong một bảng hay không (vì nó có thể đã bị xóa). Nếu có, nó sẽ xóa toàn bộ bảng khỏi tài liệu cũng như đoạn trước nó miễn là nó được định dạng với kiểu tiêu đề, ví dụ: "Heading 1".

**Ví dụ**

Hiển thị cách xác định logic tùy chỉnh trong trình xử lý triển khai IFieldMergingCallback được thực thi cho các vùng chưa được hợp nhất trong tài liệu.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-EmptyRegionsHandler.java" >}}

Kết quả của mã trên được hiển thị bên dưới. Các trường chưa được hợp nhất trong khu vực đầu tiên được thay thế bằng văn bản thông tin và việc xóa bảng và tiêu đề cho phép tài liệu trông hoàn chỉnh.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-2](how-to-apply-custom-logic-to-unmerged-regions-3.png)


Mã loại bỏ bảng cha cũng có thể được thực hiện để chạy trên mọi vùng không sử dụng thay vì chỉ một vùng cụ thể bằng cách xóa kiểm tra tên bảng. Trong trường hợp này, nếu bất kỳ vùng nào bên trong bảng không được hợp nhất với bất kỳ dữ liệu nào, cả vùng và bảng vùng chứa cũng sẽ tự động bị xóa.

Chúng ta có thể chèn mã khác nhau trong trình xử lý để kiểm soát cách xử lý các vùng chưa được hợp nhất. Thay vào đó, sử dụng mã bên dưới trong trình xử lý sẽ thay đổi văn bản trong đoạn đầu tiên của khu vực thành một thông báo hữu ích trong khi bất kỳ đoạn tiếp theo nào trong khu vực đều bị xóa. Các đoạn văn khác này bị xóa vì chúng sẽ vẫn còn trong khu vực sau khi hợp nhất thông điệp của chúng tôi.

Văn bản thay thế được hợp nhất vào trường đầu tiên bằng cách đặt văn bản được chỉ định vào thuộc tính **FieldMergingArgs.Text**. Văn bản từ thuộc tính này được hợp nhất vào trường bởi công cụ Mail Merge.

Mã này chỉ áp dụng cho trường đầu tiên trong khu vực bằng cách kiểm tra thuộc tính **FieldMergingArgs.FieldValue**. Giá trị trường của trường đầu tiên trong khu vực được đánh dấu bằng "FirstField". Điều này làm cho loại logic này dễ thực hiện hơn nhiều khu vực vì không cần thêm mã.

**Ví dụ**

Cho thấy làm thế nào để thay thế một khu vực không sử dụng với một tin nhắn và loại bỏ các đoạn phụ.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-ReplaceAnUnusedRegionWithAMessage.java" >}}

Tài liệu kết quả sau khi mã trên đã được thực thi được hiển thị bên dưới. Vùng không sử dụng được thay thế bằng thông báo cho biết không có bản ghi nào để hiển thị.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-3](how-to-apply-custom-logic-to-unmerged-regions-4.png)


Ví dụ khác, chúng ta có thể chèn mã bên dưới thay cho mã ban đầu xử lý **SuppliersRegion**. Thao tác này sẽ hiển thị một thông báo trong bảng và hợp nhất các ô thay vì xóa bảng khỏi tài liệu. Vì khu vực nằm trong một bảng có nhiều ô, nên việc các ô của bảng được hợp nhất với nhau và thông báo được căn giữa sẽ đẹp hơn.

**Ví dụ**

Hiển thị cách hợp nhất tất cả các ô mẹ của một vùng không sử dụng và hiển thị thông báo trong bảng.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-MergeAllTheParentCellsOfAnUnusedRegion.java" >}}

Tài liệu kết quả sau khi mã trên đã được thực thi được hiển thị bên dưới.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-4](how-to-apply-custom-logic-to-unmerged-regions-5.png)


Cuối cùng, chúng ta có thể gọi phương thức **ExecuteCustomLogicOnEmptyRegions** và chỉ định tên bảng cần được xử lý trong phương thức xử lý của chúng tôi, trong khi chỉ định các tên khác sẽ tự động bị xóa.

**Ví dụ**

Chỉ ra cách chỉ định vùng `ContactDetails` được xử lý thông qua lớp handler.

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e" "Examples-src-main-java-com-aspose-words-examples-mail_merge-ApplyCustomLogicToEmptyRegions-HandleTheContactDetailsRegion.java" >}}

Gọi quá tải này với ArrayList được chỉ định sẽ tạo nguồn dữ liệu chỉ chứa các hàng dữ liệu cho các vùng được chỉ định. Các khu vực khác ngoài khu vực `ContactDetails` sẽ không được xử lý và sẽ tự động bị xóa bởi động cơ Mail Merge thay thế. Kết quả của cuộc gọi trên bằng cách sử dụng mã trong trình xử lý ban đầu của chúng tôi được hiển thị bên dưới.

![apply-custom-logic-to-unmerged-regions-aspose-words-java-5](how-to-apply-custom-logic-to-unmerged-regions-6.png)
