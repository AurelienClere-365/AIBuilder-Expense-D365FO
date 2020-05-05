# AIBuilder-Expense-D365FO
AI Builder Text Recognition Expenses with Dynamics 365 FinOps


Sample PowerAutomate flows in order to create automatically Expenses in Dynamics 365 Finance and Operations with the AI Builder of the PowerPlatform.


1/ You will need a Trial or license of AI Builder

2/ Import also the Data Entity (IMPExpTransV2) in your Dynamics 365 FinOps tenant

3/ Import first the childflow

4/ Import the main flow AI Builder + change the URL of the last call at the end of the flow with the generated URL coming from the child flow before.

5/ See if you have a worker assigned in your Systemuser account in Dynamics365 FinOps, as well as a manager with HR module with job positions hierarchies.

6/ Test it with like the example of the expense attach in this github project.


DISCLAIMER :
It's just a proof of concept, and don't use it (yet) in production environment. It's just a demonstration and you will need to change/improve based on the use case you want to achieve.

Improvements :
=> Ask for a project in the input of the Flow (if you want to have a relationshipt between a project in FinOps and the expense of the end user)
=> Detect automatically the category of the expense (at this time I put hard coded TEST)
=> Attach the expense with DocuRef entity after uploading in your sharepoint repository.
=> Improve the delimiter for the Transaction Date and Total Amount + Currency based on your template of expense in your country.

See the article on my blog for more details : https://www.powerazure365.com/blog-1/ai-builder-powerplatform-for-expense-management-in-dynamics-365-finance-and-operations
