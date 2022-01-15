---
title: Item documents in Russia
description: Russian enhancements include item documents.
author: DianaMalina

ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords:
ms.date: 04/01/2020
ms.reviewer: edupont
ms.author: soalex
---

# Item Documents

[!INCLUDE[prodshort](../../includes/prodshort.md)] includes several documents that you can use to manage your warehouse. This also includes reports that you must submit for official reporting, such as the Item Report TORG-29, Items Receipt Act TORG-1, and Receipt Deviations TORG-2 reports.

The following types of documents are useful for managing your warehouse:

- Item receipt act without the vendor invoice - This is applied to the account receipt of items based on the quality, quantity, and cost.
- Item writing-off act – This is applied to register damage for reasons such as the loss of quality of items that will no longer be sold.
- Item transfer – This is applied to receipt and delivery shipments for transfer of items within the organization.

## Setting Up Warehouse Document Numbering

The following procedure shows how to set up warehouse document numbering.

1. Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Setup**, and then choose the related link.
2. On the **Numbering** FastTab, specify in the following fields the series of numbers for documents:
   - **Item Receipt Nos**
   - **Posted Item receipt Nos**
   - **Item Shipment Nos**
   - **Posted Item Shipment Nos**

## Creating an Item Receipt Act Without a Vendor

The following procedure shows how to create an item receipt act without a vendor.

1. Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Receipts**, and then choose the related link.

2. In the header of the **Item Receipt** window, enter the fields described in the following table.

   | Field                               | Description                                                  |
   | ----------------------------------- | ------------------------------------------------------------ |
   | **No.**                             | Specifies the warehouse document header number.              |
   | **Posting Description**             | Specifies the posting description.                           |
   | **Location Code**                   | Specifies the value code that is filled in from the Location list. |
   | **Gen. Bus. Posting Group**         | Specifies the code of the general business posting group.    |
   | **Posting Date**  **Document Date** | Specifies the working date that is filled in by default.     |
   | **External Document No.**           | Enter the primary document number.                           |
   | **Purchaser Code**                  | Specifies the value code that is selected from salespeople or purchasers. |
   | **Correction**                      | Specifies if the entry is a correction.                      |
   | **Status**                          | Specifies if the document is Open or Released.               |

3. In the document lines of the **Item Receipt** window, enter the fields described in the following table.

   | Field                      | Description                                                  |
   | -------------------------- | ------------------------------------------------------------ |
   | **Item No.**               | Specifies the item number from the Item List table.          |
   | **Description**            | Specifies the item description.                              |
   | **Quantity**               | Specifies the number of item units.                          |
   | **Reserve Quantity Inbnd** | Specifies the item quantity reserved at the warehouse of the receiver. |
   | **Unit Amount**            | Specifies the price of a unit item.                          |
   | **Indirect Cost %**        | Specifies the indirect cost percent.                         |
   | **Unit Cost**              | Specifies the item unit cost of the receipt shipment line.   |
   | **Amount**                 | Specifies the transaction amount.                            |
   | **Unit of Measure Code**   | Specifies the unit of measure code for the received items.   |

4. In the **Item Receipt** window, choose the **Employee Signatures** action to specify the signature of the person in charge.

5. Enter the fields described in the following table.

   | Field             | Description                                                  |
   | ----------------- | ------------------------------------------------------------ |
   | **Employee Type** | Specifies the type of the employee.                          |
   | **Employee No.**  | Specifies the employee number of the employee who must sign. |
   | **Employee Name** | Specifies the values that are retrieved from the standard fields of the selected **Employee Card**. |

6. To print an **Item Receipt** report from the **Item Receipt** window, choose the **Item Document** action.

7. Choose the **Print** button.

The following functions are available in the **Item Receipt** window.

| Function                         | Description                 |
| -------------------------------- | ----------------------------|
| Changing document status         | Documents can be open or released for the next processing stage. Choose the **Release** or the **Reopen** action. |
| Reservation of document lines    | Items can be reserved from the document line. Choose the **Reserve** action. |
| Warehouse adjustment calculation | Refers only to item quantity corrections in the warehouse bins. This is accessible only if advanced picking and placing is used in the warehouse. |
| Document posting                 | Choose the **Post** action to perform the following:   -   **Post** Post the item receipt. The posted item receipt is created. -   **Post and Print** Post the receipt and print the test report. |

## Analysis of a Posted Document Item Receipt Without a Vendor

The following procedure shows how to analyze a posted document item receipt without a vendor.

1. Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Item Receipts**, and then choose the related link.

   > [!NOTE]
   > The posted item receipt displays all the information from the item receipt.

2. Choose the **Sort** action to sort the list of documents selected for printing in ascending or descending order.

3. Choose the **Print** button.

## Creating an Item Writing-Off Act

The following procedure shows how to create an item writing-off act.

1. Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Item Shipments**, and then choose the related link.

2. On the header of the **Item Shipment** window, enter the fields. These fields are the same as those on the **Item Receipt** window.

3. In the document lines of the **Item Shipment** window, enter the fields. These fields are the same as those on the **Item Receipt** window except for the following:

    - The **Indirect Cost** field is available only in the **Item Receipt** window.
    - The fields in the following table are available only in the **Item Shipment** window.

    | Field                      | Description                                                  |
    | -------------------------- | ------------------------------------------------------------ |
    | **FA No.**                 | Specifies the fixed asset to write off items and materials.  |
    | **Depreciation Book Code** | Specifies the fixed asset depreciation book to which the additional cost will be added. |

4. In the **Item Shipment** window, choose the **Employee Signatures** actionm to specify the signature of the person in charge.

5. Enter the fields described in the following table.

    | Field             | Description                                                  |
    | ----------------- | ------------------------------------------------------------ |
    | **Employee Type** | Specifies the type of the employee.                          |
    | **Employee No.**  | Specifies the employee number of the employee who must sign. |
    | **Employee Name** | Specifies the values that are retrieved from the standard fields of the selected **Employee Card**. |

6. Choose the **Print** action.

The functions available in the **Item Shipment** window are same as those in the **Item Receipt** window.

## Analysis of a Posted Document Item Writing-Off Act

The following procedure shows how to analyze a posted document item writing-off act.

1. Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Item Shipments**, and then choose the related link.

  > [!NOTE]
  > The posted item shipment displays all the information from the item shipment.

2. Choose the **Sort** action to sort the list of documents selected for printing in ascending or descending order.

3. Choose the **Print** action.

## Report Transfer Order TORG-13 Based on an Unposted Transfer Document

The following procedure shows how to create a Transfer Order TORG-13 report based on transfer documents that are not posted.

1. Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transfer Orders**, and then choose the related link.

   Choose the **Print** action.

## Report Transfer Order TORG-13 Based on a Posted Transfer Document - Transfer Receipt

The following procedure shows how to create a report based on a posted transfer document called a transfer receipt.

1. Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Transfer Receipt**, and then choose the related link.
2. Choose the **Print** action.

## Report Transfer Order TORG-13 Based on a Posted Transfer Document - Transfer Shipment

The following procedure shows how to create a report based on a posted transfer document called a transfer shipment.

1. Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Transfer Shipments**, and then choose the related link.

   Choose the **Print** action.

## See Also

[Inventory Setup](Inventory-Setup.md)  
[Item Obligatory Acts](Item-Obligatory-Acts.md)  
[Item General Ledger Turnover](Item-General-Ledger-Turnover.md)  
