# Analyze and Investigate PeakGear Sales

## Introduction

In this optional lab, you will connect Oracle Smart View to the PeakGear cube, compare sales by period, product, and store, and drill through from a cube summary to the supporting Lakehouse transaction records.

Estimated Time: 25 minutes

### About Smart View and Drill-Through

Smart View lets you analyze Essbase data in Microsoft Excel. A drill-through report can show the detailed source records behind a cube value when a Lakehouse datasource and drillable region have been configured for the cube.

### Objectives

In this lab, you will:

- Connect Smart View to the PeakGear cube.
- Compare PeakGear sales across periods, products, and stores.
- Drill through from a sales value to the underlying Lakehouse detail.

### Prerequisites

This lab assumes you have:

- Microsoft Excel with a compatible Oracle Smart View for Office installation.
- The Essbase Smart View connection URL and the workshop user's Essbase credentials.
- The PeakGear cube imported with data in Lab 3.
- Access to the PeakGear sales transaction detail loaded or verified in Lab 1.
- A drill-through report configured for the PeakGear cube and its Lakehouse detail datasource.

<!-- Author TODO: Add the tested Smart View URL, the exact cube members, and the drill-through report setup or preconfiguration steps before publishing. -->

## Task 1: Connect Smart View to the PeakGear Cube

1. Open Microsoft Excel and select the **Smart View** ribbon.

2. Select **Panel**, then open **Private Connections**.

3. Enter the Smart View URL supplied for your Essbase environment. The URL ends with `/essbase/smartview`.

4. Sign in with the workshop user's Essbase credentials.

5. Expand the Essbase connection, select the PeakGear application and cube, and start an ad hoc analysis.

## Task 2: Compare PeakGear Sales

1. Place the sales measure in the grid and select a product and store member that contain data.

2. Place time periods across the columns and compare sales between two periods.

3. Zoom in on a product or store hierarchy to inspect the members contributing to a summary value.

4. Record one sales value and its selected time, product, and store members for the next task.

## Task 3: Drill Through to Lakehouse Detail

1. In the Smart View grid, select a sales cell within the configured drillable region.

2. On the **Essbase** ribbon, select **Drill-through**.

3. Review the returned PeakGear sales transaction records in the new worksheet.

4. Confirm that the records correspond to the time, product, and store members selected in the cube.

    > **Note:** If **Drill-through** is unavailable or returns no records, verify that the PeakGear detail source and drill-through report are configured for the selected cell.

You have compared PeakGear sales in Smart View and investigated a cube value using Lakehouse transaction detail.

## Learn More

- [Analyze an Application in Smart View](https://docs.oracle.com/en/database/other-databases/essbase/26/esscd/top-tasks-oracle-essbase.html)
- [Introduction to Essbase Drill Through](https://docs.oracle.com/en/database/other-databases/essbase/26/ugess/introduction-essbase-drill-through.html)
- [Test Drill Through Reports](https://docs.oracle.com/en/database/other-databases/essbase/21/ugess/test-drill-reports.html)

## Acknowledgements

* **Author** - Ty Wolber, Cloud Engineer
* **Last Updated By/Date** - Ty Wolber, October 2026
