#### **innerRangePadding** : {<%= type %>}

<% if(defaultValue !== "[object Object]") { %>*default: <%= defaultValue %>* <% }%>

This property only applies to [column](#column) and [bar](#bar) visualizations.

In column visualizations, the amount of whitespace (padding) between the columns, expressed as a percentage of the range band. (The range band is the distance between the edges of a single column of data, and is based on dividing the entire domain into evenly spaced intervals.)

**Example:**

    new Contour({
        el: '.myColumnChart',
        xAxis: { innerRangePadding: 0.9 }
      })
    .cartesian()
    .column(data)
    .render()

*[Try it.](<%= jsFiddleLink %>)*

**Notes:**

Use the [`outerRangePadding`](#config_config.xAxis.outerRangePadding) to set the amount of whitespace between the first (and last) column and the edge of the axis.
