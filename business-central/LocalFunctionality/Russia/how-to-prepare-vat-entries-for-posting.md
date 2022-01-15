---
title: Preparing VAT entries for posting in Russia
description: Russian enhancements include periodically remit the net VAT from sales and purchase transactions to the tax authorities.
author: DianaMalina

ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords:
ms.date: 04/01/2020
ms.reviewer: edupont
ms.author: soalex
---

# Prepare VAT Entries for Posting

You may want to periodically remit the net VAT from sales and purchase transactions to the tax authorities. You can use the **VAT Settlement Worksheet** to prepare transactions with open VAT amounts for posting and copy the entries to the appropriate VAT settlement journal. This is typically done before you run the **Calc. and Post VAT Settlement** batch job to post and close VAT entries.

## To prepare VAT entries for posting

1. Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **VAT Settlement Worksheet**, and then choose the related link.

2. Select the filters that define the VAT related transactions that you want to include in the VAT settlement.

   | Field       | Description                                                  |
   | :---------- | :----------------------------------------------------------- |
   | **Type**    | Select the type of transactions that you want to include in the VAT settlement. |
   | **View by** | Select the time period for the VAT settlement.               |
   | **View as** | Select how you want to view the net VAT. The options include **Net Change** and **Balance at Date**. |

3. Choose **Suggest Documents**. Transactions with open VAT entries that match the filters that you selected will be displayed.

4. Review the transactions that are included to ensure accuracy. If necessary, adjust your filter selection.

5. Choose **Copy Lines to Journal**.

The entries are copied to the appropriate VAT settlement journals. You can now run the **Calc. and Post VAT Settlement** batch job to close the VAT entries.

## See Also

[Report VAT to Tax Authorities](../../finance-how-report-vat.md)  
