---
title: Posting tax differences in Russia
description: Russian enhancements include tax differences.
author: DianaMalina

ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords:
ms.date: 04/01/2020
ms.reviewer: edupont
ms.author: soalex
---

# Post Tax Differences

The **Tax Difference Journal** is used to create and post tax difference transactions. Tax differences are variations in tax amounts caused by the different rules for recognizing income and expenses between entries for book accounting and tax accounting.

You can use the **Tax Difference Journal** window to manually create tax difference journal entries or you can modify existing entries created by periodic tax difference calculation activities. When you post the **Tax Difference Journal** window, tax differences entries are posted to the selected posting groups.

## To post tax differences

1. Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Tax Difference Journals**, and then choose the related link.

2. Fill in the fields as described in the following table.

   | Field                    | Description                                                  |
   | :----------------------- | :----------------------------------------------------------- |
   | **Posting Date**         | Enter the transaction date.                                  |
   | **Document No.**         | Enter the document number from the source transaction.       |
   | **Description**          | Enter a description for the transaction.                     |
   | **Tax Diff. Type**       | Select if the tax difference is **Constant** or **Temporary**. |
   | **Tax Diff. Code**       | Select an identifying income or expense code that defines the source of the tax difference. |
   | **Source Type**          | Select the source of tax difference. The options include **Future Expense**, **Fixed Asset**, and **Intangible Asset**. |
   | **Source No.**           | If the **Source Type** is **Future Expense**, enter an identifying code for the future period expenses.  Otherwise, leave this field blank. |
   | **Jurisdiction Code**    | Select the identifying code for the jurisdiction that is used to calculate taxable profits and losses for tax differences. |
   | **Norm Code**            | Select the identifying code for the norm jurisdiction that is used to calculate taxable profits and losses for the tax differences. |
   | **Tax Factor**           | Enter the profit tax rate that is used to calculate tax differences. |
   | **Amount (Base)**        | Enter an expense amount based on book accounting transactions. This information is used if the tax difference calculation is for a set period of time. |
   | **Amount (Tax)**         | Enter an expense amount based on tax accounting transactions. This information is used if the tax difference calculation is for a set period of time. |
   | **Difference**           | Enter the value of the difference between the book accounting and tax accounting transactions. |
   | **YTD Amount (Base)**    | Enter the year-to-date value of the expense or income amount based on the book accounting data. |
   | **YTD Amount (Tax)**     | Enter the year-to-date value of the expense or income amount based on the tax accounting data. |
   | **YTD Difference**       | Enter the year-to-date value of the difference between the book accounting and tax accounting transactions. |
   | **Tax Diff. Calc. Mode** | Specifies the difference of the counting mode. If **Balance** is selected, the difference will be calculated by a creating total starting from the start of the year. If not selected, the difference will be created for the current period. |
   | **Tax Amount**           | Specifies the counting result. The value of this field will correct the profit tax in the book accounting transactions. |
   | **Asset Tax Amount**     | Specifies the calculated asset tax amount.                   |
   | **Liability Tax Amount** | Specifies the calculated liability tax amount.               |
   | **Disposal Tax Amount**  | Specifies the tax amount that is written off at disposal of an item. |
   | **DTA Starting Balance** | Specifies the starting disposal tax amount before counting.  |
   | **DTL Starting Balance** | Specifies the starting disposal tax liability amount before counting. |
   | **DTA Ending Balance**   | Specifies the disposal tax amount after counting.            |
   | **DTL Ending Balance**   | Specifies the disposal tax liability amount after counting.  |
   | **Disposal Mode**        | Select if you want to write down the tax difference or transform it into a constant difference. |
   | **Disposal Date**        | Enter the date of the item’s disposal.                       |
   | **Partial Disposal**     | Select if you want to dispose of an item that causes differences in the expense or income code. If this field is not selected, the tax differences are written off. |

3. Choose the **Post** action. The tax difference journal transaction is posted.

4. Choose the **Ledger Entries** action to open the **Tax Diff. Ledger Entry** window and review the posted entries.

## See Also

[Tax Differences](Tax-Differences.md)  
[Setting up Tax Difference Calculation](Setting-up-Tax-Difference-Calculation.md)  
[Tax Accounting](Tax-Accounting.md)  
[Tax Registers](Tax-Registers.md)  
[Create Tax Registers](How-to-Create-Tax-Registers.md)  
