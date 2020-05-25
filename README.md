# Tableau_DS

https://zhuanlan.zhihu.com/p/61105327?utm_source=wechat_session&utm_medium=social&utm_oi=978141281302552576
-  Parameter action
		a. Create parmeter,
		b. Add parameter action (worksheet>add action > change parameter)
    c. Assign action
- Parameter Action: when selected, assign field to the target parameter

- AVG function ignores null values
- An aggregated calculation can be multiplied by a non-aggregated constant.

- Dimensions come out to view by themselves , measures are aggregate; discrete are blue, continuous are green

- As for data blending, it is used when you blend data from multiple data sources on a single worksheet. For each data source that is used on the sheet, a query is sent to the database and the results are processed. Then all the results are left joined on the common dimensions.(which means that you must define common dimensions between the primary and secondary data sources )

- Twbx. Doesn't create an extract of the data, but can contain both live connections and/or data extracts


- Data Source filter >> context filter

- Tree map: color, size, detail

- MEASURE and DIMENSION are NOT about colors.
- DISCRETE and CONTINUOUS relate to COLOR
- Text and Boolean values are ALWAYS DISCRETE and cannot be converted to continuous
- DATE fields can be CONTINUOUS or DISCRETE
- You CANNOT make a type conversion between a MEASURE and a DIMENSION if you are connected to a CUBE data source
- You CAN change the geographic roles of a DIMENSION
- Shape and Sort are default properties only for DIMENSIONS
- SORT can NOT break the dimension hierarchy
- MEASURE does NOT change the granularity of the view
- Only DIMENSION changes the granularity of the view
- MEASURE over time is displayed as a LINE
- You can add more than 1 worksheet to a TOOLTIP
- You CANNOT add dashboards to a TOOLTIP
- A TOOLTIP worksheet is not dynamic
- You can edit a TOOLTIP worksheet
- If you cant edit an AXIS it is because it is a LABEL (a discrete measure)
- TREE MAPS do not have column or row shelves
- You CAN combine static and dynamic SETS
- You CAN create a group from another GROUP
- You CANNOT create a GROUP from a SET
- You CANNOT create a SET from a set
- SETS can ONLY be used on dimensions
- SETS are DYNAMIC and groups are NOT
- SETS ENCAPSULATE members, groups MERGE them into a single label
- SETS do NOT create a DISCRETE dimension
- You CAN assign custom territories using GROUP and assigning it as a geographic field,
- NOT with a SET.
- You can NOT create a dynamic SET by selecting marks in the view.
- You can use a field as a FILTER even if that field is not in the view
- The ORDER of pills on the filter shelf does not affect the result
- The pill gets a grey color when you add it CONTEXT
- You can NOT have a live connection for salesforce
- You can ONLY have a live connection for cubes
- You CANNOT union tables if they come from a different data connection
- In a single database JOIN your data source contains one connection
- A cross DB join contains 2 data connections
- BLENDING has two data sources and one connection per data source
- BLENDING requires a common DIMENSION
- Be aware of different AGGREGATES when using joins
- Data from splits can be used for BLENDING. NOT joins.
- FIXED and INCLUDE consider the dimensions in the view
- FIXED can result in a DIMENSION or a MEASURE
- INCLUDE and EXCLUDE always result in a MEASURE
- FIXED is executed before INCLUDE and EXCLUDE
- HISTOGRAM uses BIN DATA
- Measures do NOT affect the granularity of the view
- Partitioning defines the SCOPE
- Addressing defines the DIRECTION
- Spatial files are useful to show shapes INCLUDING highways, they CANNOT show measures.
- Spatial data supports POINT, LINEAR, POLYGON geometries
- Click on linear TREND LINE to access exponential trend line
- TREND lines are per PANE or per COLOR
- TREND lines can only be used with numeric or date fields
- BOX PLOTS: IQR = upper hinge – lower hinge
- It is DEVICE PREVIEW when designing a device layout
- A STORY consists of sequential story points
- The metadata grid does NOT display the fields in your data source in columns
- Remember to use worksheets as filters when searching in dashboard data
- AVG is an aggregation function and ignores null values
- You CANNOT aggregate more than once
- You CANNOT mix aggregate and non-aggregate fields in your calculated field.
- Below window AVG – WINDOW_AVG(SUM([Profit])) – SUM([Profit])
- Mark annotations stay with the mark
- Point annotations stay at the same point in the view
- Point annotations are independent of the mark
- Area annotations can show outlier values
- An aggregated calculation can be multiplied by a non-aggregated constant
- Use Tableau Reader to send if they do not have Tableau Desktop
- Blending requires a common DIMENSION
- Joins require a common Column ID
- Target Diff = Sum(Target) – sum(Sales)
- To get % = Target Diff / sum(Sales)
- Profit Ratio – Profit / Sales
- BULLET CHART -> TARGET of 10% = Sales * 0.1
- Place Target on detail
- P-Value represents SIGNIFICANCE
- P-Value needs to be IF [Status] = ‘Returned’ THEN 0 ELSE [Sales] END
- FORECAST to grow 50% -> sum(Sales) * 1.5
- Go to URL does NOT have target sheets
- FILTER and HIGHLIGHT have target sheets
- HIGHLIGHT action CAN be applied to an entire workbook
- HIGHLIGHT action in a dashboard is not similar to FILTERING
- Best reason for using an EXTRACT instead of a LIVE connection is when you need to apply an aggregation. LIVE takes too long
- A REFERENCE DISTRIBUTION plot CAN be on a continuous axis
- A REFERENCE BAND is placed on two reference points
- A WMS service helps for geo-referenced map images and aids in map visualization
- A sheet CAN be used directly in a story
- Calculated fields are used for creating variable BIN sizes
- A BULLET GRAPH compares the actual sales with the targeted sales
- GANTT CHART needs a DURATION
- 32GB is recommended for Tableau SERVER
- DATA SERVER is useful for publishing a data source and creating new workbooks.
- SUBSCRIBE users by clicking subscribe on the view then add under subscribe others
- Manage PERMISSION on the workbooks permission page then click PERMISSION rules
- Join type for BLENDED data is LEFT JOIN
- Extract filters >> Data Source filters >> Context filters >> LOD Fixed >> Dimension filters >> LOD Include/Exclude >> Measure filters >> Table calc filters
