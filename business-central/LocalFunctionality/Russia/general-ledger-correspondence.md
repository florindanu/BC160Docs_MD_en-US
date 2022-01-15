---
title: General ledger correspondence in Russia
description: Russian enhancements include G/L correspondence.
author: DianaMalina

ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords:
ms.date: 04/01/2020
ms.reviewer: edupont
ms.author: soalex
---
# General Ledger Correspondence

The general ledger correspondence feature enables you to: 

- Create a correspondence transaction periodically.
- Post correspondence operations when you post general ledger transactions.
- Analyze a number of reports for correspondence.

## Creating a General Ledger Correspondence Entry

The following procedure shows how to periodically create general ledger correspondence entries.

1. Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Create G/L Correspondence**, and then choose the related link.
2. Enter the **Transaction No.** field with the transaction number if general ledger correspondence is to be created only for the selected transaction. Otherwise, leave it blank.

To set up automatic general ledger correspondence:

1. Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Ledger Setup**, and then choose the related link.
2. Select the **Automatic G/L Correspondence** check box.

## Reports

The following reports have been added for the analysis of data from correspondence transactions:

- General Ledger - Correspondence (page 12403; report 12431)
- G/L Correspondence Entries (page 12401)
- G/L Corresp. Journal Order (report 12432)
- G/L Corresp Entries Analysis (report 12435)

### General Ledger - Correspondence Window

The **General Ledger - Correspondence** window shows turnovers in the chosen period in correspondence.

1. Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Correspondence**, and then choose the related link.
2. Choose the **General Ledger - Correspondence** action.

The header of the **General Ledger - Correspondence** window contains the following filters:

- Date Filter
- Business unit Filter
- Global Dimension 1 Filter
- Global Dimension 2 Filter

In the subform, the report shows the turnover in correspondence with other accounts:

:::image type="content" source="../../media/ru/General-Ledger-Correspondence.png" alt-text="General ledger correspondence":::

### G/L Corresp Entries Analysis Report

The **G/L Corresp Entries Analysis** report shows the correspondence entries for each account. The report can be used to get an overview of general ledger account entries with correspondence and totals.

1. Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Correspondence**, and then choose the related link.
2. Choose the **G/L Corresp Entries Analysis** action.

On the **Options** tab of the request form, you can set parameters by filling in the fields with the information listed in the following table.

| Field                  | Description                                                  |
| ---------------------- | ------------------------------------------------------------ |
| **Period Beginning**   | Enter the starting date of the period, for the entries that you want to include in the report. |
| **Ending of Period**   | Enter the ending date of the period, for the entries that you want to include in the report. |
| **Other parameters**:<br />**Without Zero Net Changes**, **Without Zero Lines**, **Debit Credit Separately**, **New Page for GL Acc** | Specify the view of the report, such as whether the information for each account should be written without zero lines or net changes. |

## See Also

[Russia Local Functionality](russia-local-functionality.md)
