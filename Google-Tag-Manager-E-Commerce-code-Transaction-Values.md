## Transaction data

GTM Data layer | Name | Sample | Required | Value Type | Additional comment
---------------|------|--------|----------|------------|-------------------
transactionId|Transaction / order ID|12345|Yes|string| |
transactionAffiliation|Affiliation / Shop name|Webshop|No|string|Optional for specific shopversions
transactionTotal|Total order value|53.30|Yes|decimal _5,2_|Order total including VAT. Currency values should always use a dot "."
transactionTax|VAT|15.99|Yes|decimal _5,2_|Currency values should always use a dot "."
transactionShipping|Shipping cost|4.99|Yes|decimal _5,2_|Currency values should always use a dot "."
transactionPaymentType|Payment Type|CreditCard &#124; VISA|No|string|Payment type and financial service provider. Seperated by "&#124;" (pipe)
transactionCurrency | Currency in which the transaction is fulfilled|EUR|Yes|string|For currency codes please refer to the [Google Developers site](https://developers.google.com/analytics/devguides/platform/features/currencies)
transactionPromoCode|Coupon / promotional code|Summer_sale_13|No|string|
transactionProducts||gtm_products|Yes||**Don't not alter**


## Product data

GTM Data layer | Name | Sample | Required | Value Type | Additional comment
---------------|------|--------|----------|------------|-------------------
sku|Product ID / SKU|962829|Yes|string| |
name|Product name|Brown jacket &#124; Hugo Boss|Yes|string|Product name and brand. Seperated by "&#124;" (pipe)
category|Product category|Jackets &#124; Men|Yes|string|Product category and optional parent category. Seperated by "&#124;" (pipe)
quantity|Number of products|3|Yes|integer|
price|Product price|50.00|Yes|decimal _5,2_|Price per item. Currency values should always use a dot "."
