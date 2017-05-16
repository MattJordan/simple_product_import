# reaction-product-importer
Product Importer allows you to bulk upload products from a CSV file. Each CSV requires a column called ProductId that groups variants together. 
Then you make the second level variant whatever you want and the third variant whatever you want. 
You can also control the mapping from one column to a corresponding DB field, or name your columns to correspond

Here's an example of what basic csv import file could look like:

| productId | topProductType | productTitle           | pageTitle                                          | vendor               | handle          | variantTitle          | variantType | title                | optionTitle | price | qty | weight | taxable | hastags               | metatags                           | description                                                                        |
|-----------|----------------|------------------------|----------------------------------------------------|----------------------|-----------------|-----------------------|-------------|----------------------|-------------|-------|-----|--------|---------|-----------------------|------------------------------------|------------------------------------------------------------------------------------|
| 1         | simple         | Basic Reaction Product | This is a basic product. You can do a lot with it. | Example Manufacturer | example-product | Basic Example Variant | variant     | Option 1 - Red Dwarf | Red         | 19.99 | 19  | 35     | true    | Hashtags, Womens, Red | Material=Cotten, Quality=Excellent | Sign in as administrator to edit.You can clone this product from the product grid. |


The plugin also includes a button to generate a sample.

### What kind of fields does Product Importer support?
- top level - there are certain fields that only apply to top level products (topProductType, pageTitle, handle, hastags, metafields, description) these need to be on the first of each product but can be filled out for each item.
- hashtags - each hashtag (tag) need to be separated by a ,
- metafields - each key value pair need to be separated by , and each key needs to be separated from value by =
- Custom Arrays - can be split by whatever symbol you enter into the delimiting field
- Custom Objects - can be delimited by any field but key values must be separated by =



