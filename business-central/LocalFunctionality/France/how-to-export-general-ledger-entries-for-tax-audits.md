---
    title: How to Export General Ledger Entries for Tax Audits
    description: This topic describes how to prepare audit files to comply with tax regulations in France.
    author: sorenfriisalexandersen

    ms.service: dynamics365-business-central
    ms.topic: article
    ms.devlang: na
    ms.tgt_pltfrm: na
    ms.workload: na
    ms.search.keywords:
    ms.date: 04/01/2020
    ms.author: sgroespe

---
# Export General Ledger Entries for Tax Audits
In France, companies must provide corporate tax and VAT information, such as transactions and general ledger postings, for audits in a file format that is specified by tax authorities. In [!INCLUDE[prodshort](../../includes/prodshort.md)], this information is recorded in a standard audit file that is designed to provide information about account types that include posted entries.

You can include opening balances in the file, but these are not actual posted entries. [!INCLUDE[prodshort](../../includes/prodshort.md)] calculates opening balance by using account entries up to the starting date that you specify for the file. The calculation also includes the closing entries that are generated by closing the prior year. The opening balances are mapped to the required fields in the report.  

If you do not close your fiscal year or do not run the **Close Year** action before generating the report, the file will include balances from income statement accounts.  

> [!NOTE]  
>  Opening balances are included in the report only for accounts with balances that are not equal to zero. To identify opening balances, look for the following values in the following fields:  
>   
>  -  JournalCode = 0  
> -   JournalLib = BALANCE OUVERTURE  
> -   EcritureNum = 0  
> -   EcritureLib = Accounts prefixed with BAL OUV  
> -   ValidDate = Start date specified on the report's request page  

> [!NOTE]  
>  Before exporting general ledger entries, make sure you have marked G/L Accounts to be detailed when exporting opening balances. This is usually a requirement for bank, customer and vendor G/L Accounts. This is done by enabling the checkbox in the field **Detailed Balance** on th **G/L Account Card** page.
>   

## To export general ledger entries to a text file for a tax audit  
1.  Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Export G/L Entries ??? Tax Audit**, and then choose the relevant link.  
2.  On the **Export G/L Entries ??? Tax Audit** page, on the **Options** FastTab, fill in the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**Starting Date**|Enter the date to use as the starting date for the time period to be covered by the audit.|  
    |**Ending Date**|Enter the date to use as the ending date for the time period to be covered by the audit.|  
    |**Include Opening Balances**|Select if you want to include opening balances in the audit report file. The balances are calculated as of the date before the first date of the period covered by the report.|  

3.  Choose the **OK** button to export the file.  

When you create the report, [!INCLUDE[prodshort](../../includes/prodshort.md)] sorts the information in the report by the **No.** and **Creation Date** fields in the general ledger register.  

The report will have the following name: <taxpayername>FEC<YYYYMMDD>  

## See Also  
 [Close Years](how-to-close-years.md)
