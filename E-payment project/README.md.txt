Welcome to the E-payment project built with OutSystems.

This application entails bill payment abilities for utilities, landline, internet, mobile and cable tv services.
It also support full and/or partial and payment of bills, depending on the service provider.

The E-payment application allows login with the following sample profiles:
1. Maggie Chow. Role: Administrator.
2. John Bishop. Role: Account Manager.
3. Mohamed Amin. Role: User
4. Default community provider (For developers)

The following static entities in this project are setup as follows:
1. Biller Categories: utilities, landline, internet, mobile and cable tv
2. Biller Types: Full Payment and Full and Partial Payment
3. Transaction Statuses: In Progress, Success, Failed, Cancelled.

The entities in this project are setup as follows:
1. Billers:
   a. Biller name.
   b. Description.
   c. Biller Category Id.
   d. Biller Type Id.
   e. Biller Icon image.

2. Payment Accounts:
   a. UserId.
   b. Phone Number.   
   c. Created DateTime.
   d. Masked Card Primary Account Number (PAN).
   e. Card ExpiryDate.
   f. Account ActivityStatus
   g. Encrypted PAN and CVV. 

2. Bill Transactions:
   a. Biller Id.
   b. User Id.
   c. CreatedDateTime.
   d. Transaction Status Id.
   e. Payment Account Id.
   f. AmountPaid.
   g. Amount Due.

This application supports the following pages with the following features:
1. User Dashboard:
   a. Contains card for users's total transactions.
   b. Contains card for last 4 transactions.
   c. Contains donut chart for user's total number of transactions by category.

2. Bill Payments Page of alternate card and list views of billers,
where you can commence selected bill payment and filter by name search, biller category and biller payment type.

3. User Transactions History Page listing all user transactions.

4. Billers Management Page where you can filter by name search, biller category and biller payment type.

5. User accounts Management Page listing all user accounts where you can filter by name search and delete accounts.

6. All Transactions History Page:
   a. Contains line chart for all transactions by date.
   b. Contains donut chart for all transactions by category.
   c. List of all transactions where you can filter by name search or by date.

The following roles and their responsibilities are as follows:

1. Administrators:
   a. Can view user dashboard.
   b. Can view Bill Payments and perform payment transactions.
   c. Can view User Transactions history.
   c. Can view billers management page and create and edit billers.
   d. Can view User Accounts management page and delete accounts.
   e. Can view All Transactions history dashboard page.

2. Account Managers:
   a. Can view Bill Payments but cannot perform payment transactions.
   b. Can view billers management page and create and edit billers.
   c. Can view User Accounts management page and delete accounts.
   d. Can view All Transactions history dashboard page.

3. Users:
   a. Can view user dashboard.
   b. Can view Bill Payments and perform payment transactions.
   c. Can view User Transactions history.






