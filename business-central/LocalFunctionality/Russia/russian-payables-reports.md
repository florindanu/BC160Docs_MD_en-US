---
title: Payables reports in Russia
description: Russian enhancements include payables reports.
author: DianaMalina

ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords:
ms.date: 04/01/2020
ms.reviewer: edupont
ms.author: soalex
---

# Russian Payables Reports

The payables report feature enables you to view the vendor general ledger turnover for general ledger accounts for finance entries with the source type Vendor on the screen and in the form of a printed report. The following reports are also provided:

- Vendor General Ledger Turnover (page 12407)
- Vendor General Ledger Turnover (report 12451)
- Vendor Accounting Card (report 12445)
- Vendor Turnover (report 12444)
- Vendor Posting Group Turnover (report 12443)
- Vendor Entries Analysis (report 12446)
- Vendor Reconciliation Act (report 14911)

## Vendor General Ledger Turnover (Page 12407)

The **Vendor General Ledger Turnover** page is an electronic window that shows the vendor turnover for general ledger accounts in the context of vendors.

To access this window, choose the **Financial Management** action, choose the **Payables** action, and then choose the **Turnover** action. This window contains all the information about a vendor's entries such as the general ledger entries with the source type Vendor with the amounts in local currency (LCY).

The lines of the window contain the information listed in the following table.

| Column                                                       | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| No.                                                          | Select this column to enter the vendor number. This column is not editable. |
| Name                                                         | Select this column to enter the vendor name. This column is not editable. |
| Vendor Posting Group                                         | Select this column to enter the vendor posting group. This column is not editable. |
| Starting Balance LCY,   Debit Amount (LCY),   Credit Amount (LCY),   Ending Balance LCY,   Net Change (LCY). | Select this column to enter the balance at the beginning and the end of the period, debit amount, credit amount, and net change for the period. All amounts are shown in the local currency.   The values of these columns are calculated for all the general ledger entries with the source type Vendor.   These columns are not editable. |

The following procedure shows how to access the window with the option for the **Vendor** action.

- Choose the **Vendor** action, choose the **Vendor G/L Turnover** action, and then choose the **Card** action (SHIFT+F5 Hot Key) to view the vendor card for the selected line.

## Vendor General Ledger Turnover Report (Report 12451)

The **Vendor General Ledger Turnover** report is used to analyze turnover as well as for analysis of the vendor account balances. It is usually printed monthly, but can be printed for any given period.

The following procedure shows how to access the **Vendor General Ledger Turnover** report.

1. Choose the **Financial Management** action, choose the **Payables** action, and then choose the **Turnover** action.
2. Choose the **Vendor G/L Turnover** action, choose the **Print** action, and then choose the **G/L Turnover** action.

The **Options** FastTab contains the fields listed in the following table.

| Field                             | Description                                                  |
| --------------------------------- | ------------------------------------------------------------ |
| **Rounding Precision**            | Select this field to choose the required rounding precision such as 0.001, 0.01, 1, or 1000. |
| **Replace zero values by blanks** | Select this field to replace zero values with blanks during printing. |
| **Skip zero lines**               | Select this field to exclude lines with zero values.         |

## Vendor Accounting Card Report (Report 12445)

The **Vendor Accounting Card** report provides the following information for all of a vendor's entries for a specific period:

- Starting balance
- Posting date
- Document number
- Description
- Net change debit
- Net change credit
- Document type
- Ending balance

This report is usually printed monthly and on the date of inventory, but can be printed for any given period.

The following procedure shows how to access the **Vendor Accounting Card** report.

1. Choose the **Financial Management** action, choose the **Payables** action, and then choose the **Turnover** action.
2. Choose the **Vendor G/L Turnover** action, choose the **Print** action, and then choose the **Vendor Accounting Card** action.

The **Vendor** FastTab of the request page contains the same fields as the **Vendor** FastTab of the **Vendor General Ledger Turnover** report. On the **Options** FastTab, you can select the **New page for Vendor** check box to print the information for each vendor on a separate page.

## Vendor Turnover Report (Report 12444)

The **Vendor Turnover** report is used to print the data about a vendor's entries for a specific period in the context of separate contracts (agreements).  The system fills in the following information about the vendor:

- Starting balance (debit or credit at the start of the period)
- Net change (debit or credit)
- Ending balance (debit or credit at the end of the period)

To access the Vendor Turnover report

Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendor Turnover**, and then choose the related link.

The **Vendor** FastTab of the request page contains the same fields as the **Vendor** FastTab of the **Vendor General Ledger Turnover** report. On the **Options** FastTab, you can specify the same format options as on the **Options** FastTab of the **Vendor General Ledger** report.

The **Options** FastTab contains the fields listed in the following table.

| Field                                      | Description                                                  |
| ------------------------------------------ | ------------------------------------------------------------ |
| **Rounding Precision**                     | Select this field to choose the required rounding precision such as 0.001, 0.01, 1, or 1000. |
| **Replace zero values by blanks**          | Select this field to replace zero values with blanks during printing. |
| **Skip accounts without net changes**      | Select this field to exclude lines without net changes within the period. |
| **Skip accounts with zero ending balance** | Select this field to exclude lines with zero ending balances at the end of the period. |
| **Skip zero lines**                        | Select this field to exclude lines with zero values.         |

## Vendor Posting Group Turnover Report (Report 12443)

The **Vendor Posting Group Turnover** report is used to print information on the vendor's entries that are accumulated in the vendor posting groups. The printed data contains the following information:

- Vendor posting group code
- Vendor posting group name
- Starting balance (debit or credit)
- Net change (debit or credit)
- Ending balance (debit or credit)

To access the **Vendor Posting Group Turnover** report

- Choose the **Financial Management** action, choose the **Payables** action, choose the **Reports** action, and then choose the **Vendor Posting Group Turnover** action.

On the **Vendor Posting Group** FastTab of the request page, you can specify the vendor posting group code or a range of vendor posting group codes, depending on whether you want to print the report for one vendor posting group, or for a range of vendor posting groups.

On the **Options** FastTab, you can specify the same format options as on the **Options** FastTab of the **Vendor General Ledger Turnover** report.

## Vendor Entries Analysis Report (Report 12446)

The **Vendor Entries Analysis** report shows the vendor's liabilities at the beginning and at the end of the period, entry analysis, and invoice discharging. The printed data contains the following information:

- Posting date
- Document number
- Document name
- Type (payment, invoice)
- Amount
- Amount closed
- Payment date

This report enables you to determine the invoice and payment interdependence, and it also shows closed entries, due invoices, partially discharged invoices, and vendor prepayment amounts.

To access the **Vendor Entries Analysis** report.

- Choose the **Financial Management** action, choose the **Payables** action, choose the **Reports** action, and then choose the **Vendor Entries Analysis** action.

On the **Vendor** FastTab of the request page, you can define the vendor number or a range of numbers, depending on whether you want to print the report for one vendor or for a number of vendors. On the **Options** FastTab, you can specify the format options listed in the following table.

| Parameter               | Description                                                  |
| ----------------------- | ------------------------------------------------------------ |
| **Starting Date**       | Select this option to specify the start date of the period.  |
| **Ending of period**    | Select this option to specify the end date of the period.    |
| **Report Currency**     | Select this option to specify the currency you want to use in the report. You can choose:   -   **Local currency** -   **Transaction currency** |
| **New Page For Vendor** | Select this option to print the data for each vendor on a separate page. |

## Vendor Reconciliation Act Report (Report 14911)

The **Vendor Reconciliation Act** report shows the payments or liabilities of the vendor. It is used for the reconciliation of mutual payments of contractors.

To access the **Vendor Reconciliation Act** report

- Choose the **Financial Management** action, choose the **Payables** action, choose the **Reports** action, and then choose the **Vendor Reconciliation Act** action.

The following levels of details are possible:

- Full Detail
- Partial Detail
- None

### Full Detail

If Full Detail is selected as the detail level, the report prints the following data for each document for the current and previous periods:

- Document number and the numbers of the documents connected with it.
- The balance on each document (debit or credit)
- Document date
- Description

The report prints the following on the right side of the window (vendor's data) if **Print Contactor Data** is active on the **Options** FastTab of the request page:

- Document amount
- Debit
- Credit

### Partial Detail

If Partial Detail is selected as the detail level, the report displays the balance on each document for the current and previous periods, but does not display the connections to the invoices, credit notes, and payments.

### None

If None is selected as the detail level, the report shows the following information for each vendor:

- The balance at the beginning of the period
- Net changes for the period
- The balance at the end of the period
- Amount of the vendor liabilities
- General managers' signatures

On the **Vendor** FastTab of the request page, you can define the vendor number or a range of numbers, depending on whether you want to print a report for one vendor or for a number of vendors.

## See Also

[Russian Receivables Reports](Russian-Receivables-Reports.md)  
[Set Up Customer and Vendor Agreements](How-to-Set-Up-Customer-and-Vendor-Agreements.md)  
