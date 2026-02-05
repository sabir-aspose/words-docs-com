---
title: Working with Charts through Shape.Chart Object
second_title: Aspose.Words for C++
articleTitle: Working with Charts through Shape.Chart Object
linktitle: Working with Charts through Shape.Chart Object
description: "Charts in details, how chart linked with Shape node in Aspose.Words for C++."
type: docs
weight: 10
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /cpp/working-with-charts-through-shape-chart-object/
timestamp: 2024-01-27-14-07-04
---

Once the chart was inserted and filled with data, you are able to change its appearance. `Shape.Chart` property contains all chart related options available through the public API.

For example, let's change the Chart title or legend behavior:

{{< gist "aspose-words-gists" "d55d8631947d283b1f0da99afa06c492" "cpp-Programming-Documents-Charts-CreateChartUsingShape-CreateChartUsingShape.cpp" >}}

The code generates the followings results:

![line-chart-aspose-words-cpp](working-with-charts-6.png)

------ 

## FAQ

1. **Q:** How can I change the chart title programmatically?  
   **A:** Use the `Chart.Title` property. Set `Chart.Title.Text` to the desired string and optionally adjust formatting via `Chart.Title.Font`. Example:  
   ```cpp
   Shape* chartShape = doc->GetChildNodes(NodeType::Shape, true)->idx(0)->Cast<Shape>();
   Chart* chart = chartShape->get_Chart();
   chart->get_Title()->set_Text(u"Quarterly Sales");
   chart->get_Title()->get_Font()->set_Size(14);
   ```

2. **Q:** How do I hide or show the chart legend?  
   **A:** The legend visibility is controlled by `Chart.Legend`. Set `Chart.Legend.Visible` to `true` or `false`. Example:  
   ```cpp
   chart->get_Legend()->set_Visible(false); // hides the legend
   ```

3. **Q:** Can I change the chart type after it has been created?  
   **A:** Yes. Assign a new `ChartType` to `Chart.Type`. For instance, to convert a line chart to a bar chart:  
   ```cpp
   chart->set_Type(ChartType::Bar);
   ```

4. **Q:** How can I modify the data series values of an existing chart?  
   **A:** Access the `Chart.Series` collection, retrieve the desired `ChartSeries`, and update its `Values`. Example:  
   ```cpp
   ChartSeries* series = chart->get_Series()->idx(0);
   series->get_Values()->Clear();
   series->get_Values()->Add(150);
   series->get_Values()->Add(200);
   series->get_Values()->Add(250);
   ```

5. **Q:** Is it possible to format the axis labels (e.g., number format, font)?  
   **A:** Yes. Use `Chart.AxisX` and `Chart.AxisY` to adjust label formatting. Example:  
   ```cpp
   chart->get_AxisX()->get_NumberFormat()->set_FormatCode(u"#,##0");
   chart->get_AxisY()->get_Font()->set_Bold(true);
   ```