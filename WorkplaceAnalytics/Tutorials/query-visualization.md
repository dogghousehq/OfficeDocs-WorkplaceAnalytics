---
# Metadata Sample
# required metadata

title: Visualize person queries
description: View query results in charts without leaving Workplace Analytics
author: paul9955
ms.author: v-pascha
ms.date: 07/17/2019
ms.topic: article
localization_priority: normal 
ms.prod: wpa
---

# Visualize person queries

Analysts can be tasked with finding ways to improve teamwork in their organization. For example, you might want to discover teams whose members regularly work longer after hours or who don't seem to have enough focus time. To help you in this task, Workplace Analytics offers the [Person query](person-queries.md), which includes a number of standard and custom metrics that can help you perform analyses of this kind.  

After you create and run a Person query, you can view its results (in the form of charts) without leaving Workplace Analytics. You can refine your results view by having the charts focus on any of the metrics that you used in the query or on any organizational data attributes that have been uploaded. These steps are described in the following sections: 

- [Visualize person queries](#visualize-person-queries)
  - [Run a query and view results](#run-a-query-and-view-results)
  - [Customize your data visualization](#customize-your-data-visualization)
  - [Optional: Create a solution plan](#optional-create-a-solution-plan)
  - [Related topics](#related-topics)

In addition to these capabilities, you still have the option of exporting results to view them in a data visualization tool such as [Power BI](../use/view-download-and-export-query-results.md#use-workplace-analytics-data-in-power-bi-excel-or-other-data-analysis-tool). 

> [!Note] 
> Your query results might indicate groups of employees that could benefit from a [solution](solutions-intro.md) plan. <!-- REPLACE WHEN SV2 RELEASES: from a [solution](solutionsv2-intro.md) plan. --> You can create such a plan by starting with the query results display. For more information, see [Optional: Create a solution plan](#optional-create-a-solution-plan).

## Run a query and view results 

**Role:** analyst 

1. Open [Workplace Analytics](https://workplaceanalytics.office.com/). If prompted, enter your work credentials.

2. Expand **Analyze**, select **Queries**, and select **Person query**.

3. Define and run a person query. For more information, see [Person queries](person-queries.md). 

4. After the query finishes, open the **Results** tab.

5. In the row of the query's results, select the **Visualize** option: 

   ![Query row with Visualize](../images/wpa/tutorials/visualize-option-results-row-4.png)

   This opens a page in the **Queries > Results** area of Workplace Analytics: 

   ![Results chart](../images/wpa/tutorials/results-interactive-data-no-selections.png)

   This interactive results page lets you use charts to explore the output of your query. To change the way these results are presented, go on to the next procedure, [Customize your data visualization](#customize-your-data-visualization).

## Customize your data visualization 

**Role:** analyst 

The following steps are all optional. You can use them to refine your view of the query results in various ways. 

1. **Modify filters and metrics.** Use the **Page settings** panel to modify the date range, the filters that are applied, the metrics that you want included in your chart, and the number of groups that are displayed. Note that the kind of chart you are viewing could affect the view options that are available to you. For more information about using these settings, see [Page settings and filters](../use/chart-types.md#page-settings-and-filters). 

2. **Change chart attributes.** Use the chart toolbar to change the chart type or the chart’s sort order. Some options are available only with certain chart types.  

3. **Investigate groups.** Select particular groups in the chart to activate options for drilling down or for excluding. The groups that you select will be reflected in both the chart display and also in the settings panel. Groups will reset if you change the chart type or the sort order.  

As you add and apply filters and select groups, the chart section of the results page updates its overview of the population that you are working with. 

## Optional: Create a solution plan  

Queries can serve as a means to identify opportunities for improvement and the groups who would benefit. Query visualization lets you find and save opportunities that you've discovered in the query results. Then, you can act on those opportunities by using them to create a plan in the **Solutions** area of Workplace Analytics. 

For more information about solutions, see [Workplace Analytics solutions](solutions-intro.md).  <!-- REPLACE WHEN SV2 RELEASES: see [Workplace Analytics solutions](solutionsv2-intro.md).  -->

**Role:** analyst 

1. While visualizing a query result, select one or more groups by clicking them in a chart. In the following example, five finance groups are selected (selected groups are shown in light gray):

   ![Query results chart with group selected](../images/wpa/tutorials/results-interactive-data-close.png)

   Note the size of the selected groups. In this case, total size of the selected groups is 71 members:

   ![Total group size](../images/wpa/tutorials/group-size-finance.png)

   The group size is important because query visualization adheres to the [minimum group size](../use/settings.md#minimum-group-size) that has been set for your organization. If you've selected a group smaller than the minimum group size, you see a warning that the "filter group is below the minimum size." 

2. After you have a group or groups selected that meet or exceed the minimum group size, select **Submit group**. 

3. On the **Set up new plan** pane, select an appropriate plan type for the group that you designated and select **Start now**. 

4. Select **Validate** to validate the selected group. Workplace Analytics displays warnings if the email addresses of plan participants are faulty or if participants' licenses are missing. <!--(For more information, see [Validation](solutions-conceptual.md#validation).)   DELETING FOR NOW BECAUSE IT'S NOT IN THE SV1 DOC. --> <!-- REPLACE WHEN SV2 RELEASES: see [Validation](solutionsv2-conceptual.md#validation).)   -->

   If validation fails, you can return to your query results and select a different group or additional groups, or start over. After any subsequent group selection, you must select **Validate** again. After validation succeeds, go to the next step.

5.	With your group validated, you can now start a solutions plan. <!-- See the [Start the plan](solutions-task.md?branch=PAS-LR-SolutionsV2#start-the-plan) section of [Solution walkthrough](solutions-task.md).   DELETING FOR NOW BECAUSE IT'S NOT IN THE SV1 DOC. --> <!-- REPLACE WHEN SV2 RELEASES: See the [Start the plan](solutionsv2-task.md?branch=PAS-LR-SolutionsV2#start-the-plan) section  --> <!-- REPLACE WHEN SV2 RELEASES: of [Solution walkthrough](solutionsv2-task.md).   -->

6.	After the plan starts and is underway, you can track its progress; for more information, see [Track programs](solutions-task.md#track-programs).  <!-- REPLACE WHEN SV2 RELEASES: see [Track plans](solutionsv2-task.md#track-plans).  --> To learn about the plan from the participants' perspective, see [The experience of plan participants](solutions-participants.md?branch=PAS-LR-SolutionsV2). 
  
<!-- REPLACE WHEN SV2 RELEASES:  see [The experience of plan participants](solutionsv2-participants.md?branch=PAS-LR-SolutionsV2).   -->

## Related topics

[Person query](person-queries.md) 

[Solution walkthrough](solutions-task.md)
<!-- REPLACE WHEN SV2 RELEASES:  [Solution walkthrough](solutionsv2-task.md)   -->