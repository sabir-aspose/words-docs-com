---
title: Lồng nhau Mail Merge Với Các Vùng trong Java
second_title: Aspose.Words cho Java
articleTitle: Lồng nhau Mail Merge Với Các Vùng
linktitle: Lồng nhau Mail Merge Với Các Vùng
type: docs
description: "Thực hiện thao tác Mail Merge với các vùng lồng nhau. Hợp nhất lồng nhau là một tính năng cho phép bạn hợp nhất dữ liệu phân cấp từ nguồn dữ liệu của bạn vào mẫu hợp nhất của bạn bằng cách sử dụng Java."
keywords: "mail merge with nested regions Java, Nested Mail Merge Regions"
weight: 10
ai_search_scope: words_java
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
url: /vi/java/nested-mail-merge-with-regions/
timestamp: 2024-01-27-14-07-04
---

Trong một số trường hợp, bạn có thể cần sử dụng nested Mail Merge với các vùng. Hợp nhất lồng nhau là một tính năng cho phép bạn hợp nhất dữ liệu phân cấp từ nguồn dữ liệu của mình vào mẫu hợp nhất để dễ dàng điền vào tài liệu của bạn. Về cơ bản, dữ liệu phân cấp được biểu diễn dưới dạng một tập hợp các mục dữ liệu và các mối quan hệ phân cấp mô tả cách các mục dữ liệu có liên quan với nhau (một mục dữ liệu là cha mẹ của một mục khác).

Aspose.Words cho phép bạn thực hiện thao tác Mail Merge với các vùng lồng nhau. Bạn có thể sử dụng tính năng này nếu bạn có nguồn dữ liệu được sắp xếp thành cấu trúc giống như cây và bạn muốn thực hiện thao tác Mail Merge để điền vào mẫu với dữ liệu phân cấp.

{{% alert color="primary" %}}

Nested Mail Merge chỉ có liên quan khi thực hiện Mail Merge với các vùng.

{{% /alert %}}

## Lồng Nhau Là gì Mail Merge

Vùng Mail Merge được gọi là lồng nhau nếu bạn có hai hoặc nhiều vùng Mail Merge trong đó một trong số chúng nằm bên trong vùng kia ở dạng phân cấp. Lưu ý rằng mỗi vùng chứa dữ liệu từ một bảng.

Ví dụ phổ biến nhất về Mail Merge lồng nhau là một thứ tự chứa nhiều mục trong đó bạn cần liên kết nhiều bảng dữ liệu và trình bày thông tin trong một mẫu.

Hình dưới đây cho thấy hai vùng lồng nhau trong đó vùng *Order* Mail Merge là cha của vùng *Item* Mail Merge.

<img src="nested-mail-merge-with-regions-1.png" alt="nested_mail_merge_with_regions_aspose_words_java" style="width:650px"/>

## Cách Xử lý Mail Merge Với Các Vùng Lồng Nhau

Dữ liệu được hợp nhất thành một mẫu có thể đến từ nhiều nguồn khác nhau, chủ yếu là cơ sở dữ liệu quan hệ hoặc tài liệu XML. Trong ví dụ của chúng tôi, chúng tôi sẽ sử dụng tệp XML để lưu trữ dữ liệu của chúng tôi và tải trực tiếp vào **DataSet**.

Aspose.Words cho phép bạn xử lý Mail Merge với các vùng lồng nhau bằng cách sử dụng các mối quan hệ dữ liệu được chỉ định trong **DataSet**. Khi đối tượng **DataSet** tải XML, nó sử dụng lược đồ được cung cấp hoặc suy ra nó từ cấu trúc của chính XML để thực hiện điều này. Từ cấu trúc này, nó tạo ra mối quan hệ giữa các bảng khi cần thiết.

Hình ảnh dưới đây cho thấy cách dữ liệu từ bảng *Order* được truyền đến các vùng hợp nhất lồng nhau sẽ được liên kết với bảng *Item*, cũng như đầu ra được tạo trong quá trình hợp nhất hoạt động.

<img src="nested-mail-merge-with-regions-2.png" alt="mail_merge_with_nested_regions_aspose_words_java" style="width:650px"/>

Như bạn có thể thấy từ tài liệu đầu ra, mỗi đơn hàng từ bảng **Order** được chèn vào mẫu hợp nhất với tất cả các mục liên quan của đơn hàng từ bảng **Item**. Thứ tự tiếp theo sẽ được chèn cùng với các mặt hàng của họ cho đến khi tất cả các đơn đặt hàng và các mặt hàng được liệt kê. Thứ tự lồng Mail Merge với các vùng trong mẫu phải khớp với các mối quan hệ dữ liệu giữa các bảng trong nguồn dữ liệu.

Ví dụ mã sau đây cho thấy cách tạo hóa đơn bằng nested Mail Merge với các vùng:

{{< gist "aspose-words-gists" "827e71ccc0b8516a3cfe247b86ce6d4e"  "Examples-src-main-java-com-aspose-words-examples-mail_merge-TypesofMailMergeOperations-NestedMailMerge.java" >}}

{{% alert color="primary" %}}

Bạn có thể tải xuống tệp mẫu của ví dụ này từ [Aspose.Words GitHub](https://github.com/aspose-words/Aspose.Words-for-Java/blob/master/Examples/Data/Mail%20merge%20data%20-%20Customers.xml).

{{% /alert %}}

## Cách Thiết Lập Quan hệ Dữ liệu Trong Nested Mail Merge với Các Vùng

Bạn cần thiết lập tất cả các mối quan hệ dữ liệu trong cấu trúc cha-con để thực thi Mail Merge lồng nhau với các vùng một cách chính xác. Bỏ qua bước quan trọng này có thể dẫn đến thất bại trong việc thực thi Mail Merge lồng nhau với các vùng.

Khi truy xuất dữ liệu cho Mail Merge lồng nhau từ tệp XML bằng phương thức **ReadXml**, các mối quan hệ sẽ tự động được tạo theo cấu trúc của tài liệu XML. Tuy nhiên, bạn cần đảm bảo rằng các mối quan hệ chính xác đã được tạo ra.

Nếu Mail Merge không hoạt động như mong đợi, thì bạn có thể cần cấu trúc lại tệp XML của mình hoặc tạo rõ ràng mối quan hệ giữa các đối tượng DataTable trong DataSet.

A `DataSet` có các bảng dữ liệu liên quan sẽ sử dụng đối tượng **DataRelation** để biểu diễn mối quan hệ cha-con giữa các bảng.

Ví dụ mã sau đây cho thấy cách thiết lập `DataRelation` giữa bảng của khách hàng và bảng của đơn hàng bằng cách sử dụng đối tượng `DataRelation`:
{{< highlight java >}}
dataSet.getRelations().add(new DataRelation("OrderToItem", orderTable.getColumns().get("Order_Id"), itemTable.getColumns().get("Order_Id"), false));
{{< /highlight >}}
