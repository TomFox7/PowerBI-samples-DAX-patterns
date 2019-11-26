## Why Data Models and DAX patterns?

A pattern is a general reusable solution to a commonly occurring problem.  Proven DAX patterns leverage immense experience across many industries and set a quality expectation.  Obviously real DAX skills are still essential to adapting these patterns to new applications.

The ideal Data Models for Power BI and DAX patterns are closely related.  DAX formulae are the simplest to author and easiest to understand when the data has been shaped into the ideal data model.

I developed the live examples below in Power BI; the original examples were only available in Excel.

Acknowledgment of main sources:
- [Analyzing Data with Power BI and Power Pivot for Excel, 2017, book by Alberto Ferrari and Marco Russo](https://www.sqlbi.com/books/analyzing-data-with-microsoft-power-bi-and-power-pivot-for-excel/)
- [Dax Patterns 2015, book by Alberto Ferrari and Marco Russo and website](https://www.daxpatterns.com/patterns/)
- A Star Schema and a SWITCH for Drill-Down Income Statement Design by Matthew Mowrey (the links are below)
- A Bill of Materials solution using Power Query (M) by Imke Feldmann (the links are below)

More about patterns for data models:
- [Data Model Patterns by Rob Ferguson](https://robferguson.org/blog/2015/04/22/data-model-patterns/)

## Use Cases for DAX patterns

![Use cases of DAX patterns](https://tomfox7.github.io/PowerBI-samples-DAX-patterns/images/DAX_Patterns&Data_Models.png)
(The correlations with particular data models are work-in-progress.)

## DAX patterns in Power BI (online)
  <style>
    iframe {
      border: 1px solid black;
      width: 800px;
      height: 506px;
    }
  </style>
  
- Basket Analysis	[explained on DAX patterns site](https://www.daxpatterns.com/basket-analysis/)
- Survey	[explained on DAX patterns site](https://www.daxpatterns.com/survey/)
- Time Patterns	[explained on DAX patterns site](https://www.daxpatterns.com/time-patterns/)
- Parameter Table	[explained on DAX patterns site](https://www.daxpatterns.com/parameter-table/)

  - Basic pattern
  
    <iframe id="iframe-pt1" title="ParameterTable-basic-pattern" importance="low" src="https://app.powerbi.com/view?r=eyJrIjoiODUxMDE4ZDgtYTczZS00NDM5LWI3YzUtMGY2ZjlmZGQ2ZWM2IiwidCI6Ijg1OTBlYTFlLTdiMjctNDJlNS04MTdmLTZjOGYzNzE5ZjMxNCJ9"></iframe>
    
    
  - Single parameter
  
    <iframe id="iframe-pt2" title="ParameterTable-single-parameter" importance="low" src="https://app.powerbi.com/view?r=eyJrIjoiNjI2MmFkNGMtODUxZC00OTMzLTlhNDUtYjMxNDI0ODI1ZmYyIiwidCI6Ijg1OTBlYTFlLTdiMjctNDJlNS04MTdmLTZjOGYzNzE5ZjMxNCJ9"></iframe>
    

  - Multiple parameters
  
    <iframe id="iframe-pt3" title="ParameterTable-multiple-parameters" importance="low" src="https://app.powerbi.com/view?r=eyJrIjoiYTAzNzk3NTAtZjY3Zi00OTMwLTg4NjYtYzdiOTgwN2ViYjczIiwidCI6Ijg1OTBlYTFlLTdiMjctNDJlNS04MTdmLTZjOGYzNzE5ZjMxNCJ9"></iframe>
    
    For another example, see [Using DAX Magic For Variable Forecasting](https://powerpivotpro.com/2018/03/using-dax-magic-for-variable-forecasting/) by Matthew Mowrey.
    
    
  - Cascading parameters
  
    (later)
    
  - Limit TopN list
  
    <iframe id="iframe-pt5" title="ParameterTable-Limit-TopN" importance="low" src="https://app.powerbi.com/view?r=eyJrIjoiNmYzNGJjMGYtNTU0Ni00N2ZiLWI2MjItMjgzMTQ4YTlkOTc3IiwidCI6Ijg1OTBlYTFlLTdiMjctNDJlNS04MTdmLTZjOGYzNzE5ZjMxNCJ9"></iframe>
    

- Cum.Total	[explained on DAX patterns site](https://www.daxpatterns.com/cumulative-total/)

  - Full pattern
  
    <iframe id="iframe-ct1" title="CumTotal-full-pattern" importance="low" src="https://app.powerbi.com/view?r=eyJrIjoiMjgzZDY2NDEtNTY3Mi00MjZlLWIxOWQtYmI4YWIzYmE0ZmFmIiwidCI6Ijg1OTBlYTFlLTdiMjctNDJlNS04MTdmLTZjOGYzNzE5ZjMxNCJ9"></iframe>
    
    
  - Example of Cum.Total in Inventory Valuation
  
    <iframe id="iframe-ct2" title="CumTotal-Inventory-Valuation" importance="low" src="https://app.powerbi.com/view?r=eyJrIjoiOTRjZjM4YzUtNGZlZC00YmFiLTk0YjktYmRmOTkzODRmNmYzIiwidCI6Ijg1OTBlYTFlLTdiMjctNDJlNS04MTdmLTZjOGYzNzE5ZjMxNCJ9"></iframe>
    

- Parent-Child	[explained on DAX patterns site](https://www.daxpatterns.com/parent-child-hierarchies/)

  - Basic pattern example
    
    <iframe id="iframe-pc1" title="Parent-Child-basic" importance="low" src="https://app.powerbi.com/view?r=eyJrIjoiYTk0ZTQ2ZTAtYzgwMi00MGJiLWJlNzEtNWU2NTE3ZjdlOTMzIiwidCI6Ijg1OTBlYTFlLTdiMjctNDJlNS04MTdmLTZjOGYzNzE5ZjMxNCJ9"></iframe>

  
  - Complete example
    
    <iframe id="iframe-pc2" title="Parent-Child-complete" importance="low" src="https://app.powerbi.com/view?r=eyJrIjoiYWE0ZTg3ZjAtMDU1YS00YzlkLWJiOGMtNjI5NmI4YzZjZmRlIiwidCI6Ijg1OTBlYTFlLTdiMjctNDJlNS04MTdmLTZjOGYzNzE5ZjMxNCJ9"></iframe>
    
  
- Bill of Materials
  
  This is not yet available on the DAX patterns website, but solutions using M queries have been made by Imke Feldmann ([The BIccountant](https://www.thebiccountant.com/)):
  - [Bill of Materials (BOM) solution in Excel and PowerBI](https://www.thebiccountant.com/2017/05/08/dynamic-bill-of-material-bom-solution-in-excel-and-powerbi/)
  - [Parent-Child Hierarchies with multiple parents in Power BI with Power Query](https://www.thebiccountant.com/2019/10/03/parent-child-hierarchies-with-multiple-parents-in-power-bi-with-power-query/)
  
  
- Budget	[explained on DAX patterns site](https://www.daxpatterns.com/budget-patterns/)
  
- Star schema with a SWITCH() of measures [explained by Matthew Mowrey on PowerPivotPro site](https://powerpivotpro.com/2018/01/star-schema-switch-drill-income-statement-design/)
  
  This is an elegant solution for financial reporting and also for comparing actual performance against a budget or forecast.
  <iframe id="iframe-sss1" title="StarSchema+Switch" importance="low" src="https://app.powerbi.com/view?r=eyJrIjoiYjA2YTg0NmYtOTUwNy00ZDQ4LWI0MzQtYTU2MTIxNmFiNWMwIiwidCI6Ijg1OTBlYTFlLTdiMjctNDJlNS04MTdmLTZjOGYzNzE5ZjMxNCJ9"></iframe>

  
- Different Granularities	[explained on DAX patterns site](https://www.daxpatterns.com/handling-different-granularities/)
- ABC Classification static	[explained on DAX patterns site](https://www.daxpatterns.com/abc-classification/)
- ABC Classification dynamic	[explained on DAX patterns site](https://www.daxpatterns.com/abc-classification-dynamic/)
- Segmentation static	[explained on DAX patterns site](https://www.daxpatterns.com/static-segmentation/)
- Segmentation dynamic	[explained on DAX patterns site](https://www.daxpatterns.com/dynamic-segmentation/)
- New & Returning Customers	[explained on DAX patterns site](https://www.daxpatterns.com/new-and-returning-customers/)
- Related Distinct Count	[explained on DAX patterns site](https://www.daxpatterns.com/distinct-count/)

  - Basic pattern example
    <iframe id="iframe-rdc1" title="Related-Distinct-Count" importance="low" src="https://app.powerbi.com/view?r=eyJrIjoiNTIyZjE3ZTgtYmE4Ni00YTEzLTlmZTEtMWZkYzdmMzU3MjIwIiwidCI6Ijg1OTBlYTFlLTdiMjctNDJlNS04MTdmLTZjOGYzNzE5ZjMxNCJ9"></iframe>
    
    
  - Complete example
  
  - Slowly Changing Dimension
  
    
- Statistical	[explained on DAX patterns site](https://www.daxpatterns.com/statistical-patterns/)

  - Average/Mean
    DAX functions: AVERAGE, AVERAGEA, AVERAGEX
  - Moving Average (basic/advanced)
  - Variance
    DAX functions: VAR.S, VAR.P, VARX.S, VARX.P
  - Standard Deviation
    DAX functions: STDEV.S, STDEV.P, STDEVX.S, STDEVX.P
  - Median (basic/advanced)
  - Mode
  - Percentile (basic/advanced)
  - Quartiles
    can be calculated using the Percentile pattern.
     
  - Linear regression
    - [Simple linear regression in DAX](https://xxlbi.com/blog/simple-linear-regression-in-dax/)
    - [Multiple Linear Regression in DAX](https://stackoverflow.com/questions/48796873/multiple-linear-regression-in-power-bi)
     
  - Pearson correlation coefficient
    - [Pearson correlation coefficient in DAX](https://xxlbi.com/blog/pearson-correlation-coefficient-in-dax/)
    - [Calculating Pearson Correlation Coefficient using DAX](https://blog.gbrueckl.at/2015/06/calculating-pearson-correlation-coefficient-dax/)
