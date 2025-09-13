# Tea Sales Dashboard

This was based on a project by Mo Chen. I adjusted the data to make it a tea sales dashboard.

![Screenshot of a comment on a GitHub issue showing an image, added in the Markdown, of an Octocat smiling and raising a tentacle.](../main/Screenshot%202025-09-13%20125746.jpg)



The workflow was as follows:

1. Bringing in data from several tables into the main table.
    - Pulling in email and customer name information from the customer's table using XLOOKUP.
    - =XLOOKUP(C2,customers!$A$1:$A$1001,customers!$B$1:$B$1001,,0)

    - Using Index and match to bring in details about the tea products.
    - =INDEX(products!$A$1:$G$49,MATCH(orders!$D2,products!$A$1:$A$49,0),MATCH(orders!J$1,products!$A$1:$G$1,0))

    - Customising the date, weights and currency.

2. Visualising the data

    - Created a pivot table with date, tea type and sales.
    - Created charts to display the data.
    - Insert timeline and slicers so users can see which tea type and quantity sold well, when it sold well and who was buying it.


