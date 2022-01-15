---
    title: Registration of Sales (EET)
    description: The entrepreneur who realizes sales to be registered has the obligation to register sales. A sale to be registered is a payment in cash, by card, or by similar means, which entails a business income and which is not exempt from registration.
    author: v-pejano

    ms.service: dynamics365-business-central
    ms.topic: article
    ms.search.keywords: CZ, Czech, local, VAT, Control Report
    ms.date: 04/01/2020
    ms.reviewer: v-pejano
    ms.author: v-pejano
---

# Registration of Sales (EET)

Registration of sales (EET) is registration of sales coming from business activities and paid in cash. Information about these transactions are sent to the tax authorities. At the time of payment is created data message and sent online to the server of Tax office. As answer from the server is message with unique transaction ID, which has to be printed on the receipt for customer.

Payment methods included in EET:

- In cash  
- By card  
- Check  
- Bill of Exchange  
- Other similar types like gift cards, coupons, bitcoin etc.  

For more information see official portal [www.etrzby.cz](http://www.etrzby.cz).  

## How it Works in [!INCLUDE[d365fin](../../includes/d365fin_md.md)]

The following sales documents are covered in [!INCLUDE[d365fin](../../includes/d365fin_md.md)]:

- Sales invoice payment  
- Payment of prepayment invoice  
- Refund sales credit memo  
- Refund of prepayment invoice  
- Cash desk receipt for sales to the G/L account (without source sales document)  

With posting of defined documents (and with defined payment method) is created EET ledger entry and based on the functionality regime is processed:

- Online – An EET entry is created and stored in [!INCLUDE[d365fin](../../includes/d365fin_md.md)]. A message to the tax authorities is generated and sent to the server. An answer from the server is processed and stored and on the customer’s receipt is printed a unique transaction ID generated by tax authorities.  
- Off-line - An EET entry is created and stored in [!INCLUDE[d365fin](../../includes/d365fin_md.md)]. On the customer’s receipt is printed a unique ID generated in [!INCLUDE[d365fin](../../includes/d365fin_md.md)] (identification of company and document). EET records are processed later by batch job.  

## Main Parts of the Feature

- EET ledger entries – the table where registered documents are stored and processed. Each record contains sales data required by the tax authorities, which is needed for printing on receipts and for data from electronic communication. New records are created automatically by posting of source documents.  
- EET service settings.  
- Certificate settings.  
- EET POS terminals – identification of registered places.  

## See Also

[Czech Local Functionality](czech-local-functionality.md)  
[Finance](../../finance.md)