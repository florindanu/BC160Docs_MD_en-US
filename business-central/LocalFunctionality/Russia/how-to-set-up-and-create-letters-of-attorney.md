---
title: Setting up and creating letters of attorney in Russia
description: Russian enhancements include creating and printing letters of attorney.
author: DianaMalina

ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords:
ms.date: 04/01/2020
ms.reviewer: edupont
ms.author: soalex
---

# Set Up and Create Letters of Attorney

The letter of attorney feature enables you to create and print a Letter of Attorney, and to also print a journal of Letters of Attorney.  

Set up numbering for open and released Letters of Attorney. Numbers for open documents are generated after a new document is created. Numbers for released documents are generated after a document is printed. This number is documented in the printing form of the document and in the Letter of Attorney journal.  

The following procedure shows how to set up the numbering for Letters of Attorney.

## To set up a letter of attorney 

1. Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchases & Payables Setup**, and then choose the related link.
2. On the **Background Posting** FastTab, fill in the **Letter of Attorney Nos.** and **Released Letter of Attorney Nos.** fields.
3. Choose the **OK** button.

The following procedure shows how to create a Letter of Attorney.

## To create a letter of attorney 

1. Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Letters of Attorney** and then choose the related link.

2. Create a new document and fill in the fields in the following table.

   | Field                      | Description                                                  |
   | :------------------------- | :----------------------------------------------------------- |
   | **Letter of Attorney No.** | Enter the number of the printed document. This number is documented in the printing form of the document and in the Letter of Attorney journal. This field is filled in automatically from the numbering series. |
   | **Employee No.**           | Enter the employee number.                                   |
   | **Employee Full Name**     | Specifies the name of the employee. The field is filled in automatically from the **Employee Card**. |
   | **Employee Job Title**     | Specifies the job title of the employee. The field is filled in automatically from the **Employee Card**. |
   | **Source Document Type**   | Enter the type of source document. You can create a Letter of Attorney (header and lines) on the basis of an existing purchase document that is not yet posted. |
   | **Source Document No.**    | Enter the source document number.                            |
   | **Buy-from Vendor No.**    | Specifies the vendor number. The field is filled in automatically from the purchase document when a source document is chosen. You can manually choose the vendor. |
   | **Buy-from Vendor Name**   | Specifies the name of the vendor. The field is filled in automatically from the **Vendor Card**. |
   | **Document Description**   | Specifies information about the source document. The field is filled in automatically, but you can also manually enter the document description. |
   | **Realization Check**      | Specifies the document that is realized.                     |
   | **Document Date**          | Enter the date of the Letter of Attorney. This field is filled in with the work date by default. Manually enter the date of the document, if needed. |
   | **Validity Date**          | Enter the validity date of the document. This field is filled in by default, with the date that occurs 15 days after the document date. Manually enter the validity date, if needed. |
   | **Status**                 | Specifies the status of the document.                        |
   | **No.**                    | Enter the number of the open document. This field is filled in automatically from the numbering series. |

3. Choose the **OK** button.

## See Also

[Set Up Responsible Employees and Advance Statements](How-to-Set-Up-Responsible-Employees-and-Advance-Statements.md)  
