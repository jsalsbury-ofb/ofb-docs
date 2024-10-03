# Getting Started

## Getting Access to Classy

If you do not have access to our Classy platform, or if you are unsure, contact your supervisor or database administrator. They will provide your credentials, or create them if they do not already exist.

## Classy Gift Reports

Before you can download the gift data and import it into a Raiser's Edge batch, you will need to follow the below instructions to properly configure your Classy reports and exports so they can be handled by our macro.

### One-Time Classy Gifts

#### Setting Up One-Time Gift Reports

1. Navigate to the Classy admin page and sign in.
2. Navigate to **General Rports** and click **My Reports**.
3. Open the *One-Time Classy Gifts v8* report.
    1. If it is your first time doing this process, save a copy of the report template by clicking **Add to my Reports**.
    2. Verify that the `Report Name` is entered as *One-Time Classy Gifts v8*.
    3. The page should refresh and show this new report.
    4. **Note:** this is YOUR individual report, if changes are made and saved, it will not affect the report for others.
4. If this is your first time, ensure that you have the following *required* columns in your report to export the data properly:

??? success "Required columns for classy report"

    - Transaction ID
    - Payment Processor Reference ID
    - Transaction Date
    - Supporter Name
    - Number of Tickets
    - Gross Transaction Amount
    - Total Fees
    - Billing Email Address
    - Billing Address 2
    - Billing City
    - Billing State
    - Billing Postal Code
    - Billing Country
    - Billing Phone Number
    - Donor is Anonymous
    - Internal Campaign Name
    - Campaign ID
    - Donor’s Comment
    - Credit Card Type
    - CC Exp Date
    - Payment Type
    - Payment Processor
    - Transaction Status
    - Program Designation
    - Program Designation ID
    - Fundraising Page Name
    - Fundraiser First Name
    - Fundraiser Last Name
    - Fundraiser Supporter ID
    - Fundraising Page ID
    - Fundraising Team Name
    - Fundraising Team ID
    - Net Transaction Amount
    - Discount Amount
    - Offline Description
    - Offline Check #
    - Offline Payment Type
    - Recurring Plan ID
    - Dedication Type
    - Dedication Name
    - Dedication Message
    - Dedication Contact Name
    - Dedication Contact Email
    - Dedication Contact Address
    - Dedication Contact City
    - Dedication Contact State
    - Dedication Contact Postal Code
    - Dedication Contact Country
    - Include Donation Amount
    - Company/Organization
    - Source Code 1
    - Source Code 2

??? info "What is a one-time Classy gift?"

    A one-time Classy gift is a single, non-recurring donation made through the Classy platform. Donors can contribute a specific amount to support a fundraising campaign or cause without committing to ongoing contributions. One-time gifts are typically made via credit card, debit card, or other payment methods supported by Classy, and they provide immediate financial support for our initiatives.

#### Exporting One-Time Gifts Data

1. Open the *One-Time Classy Gifts v8* report.
2. Set the **Transaction Date** range. *Note: see "Selecting the correct Classy transaction date range" below about determining the transaction date, if this is your first time.*
3. **Note:** The Filters, Columns, and Custom Questions do not need to be changed per export - these reflect our ImportOmatic profile to import Classy data into RE. If/When the ImportOmatic profile is updated, these fields will also need to be updated accordingly.
    1. **Filters = Recurring Plan ID** is blank (only one-time gifts) and **Internal Campaign Name** is not equal to MBG (Mudbone Grown has a separate export as its one of our Fiscal Sponsor entities).
    2. **Columns = 56 options** selected to match the Excel Macro and our import profile.
    3. **Custom Question** = the additional Org question that Classy introduced outside of the *Columns* option.
4. **Save Changes** after dates are applied.
5. Export the report by clicking the small download icon at the top right portion of the Classy window. The correct button has a tooltip that reads "Export report as .CSV" for reference.
6. A pop up "Export data as .CSV file" pop up window will appear. In the `Select a specific timezone` field, verify that *Pacific Daylight Time - Los Angeles* is selected (should be by default).
7. Click **Start Export**.
8. When saving the file, use the naming convention: *MM.DD.YY - MM.DD.YY - Classy 1x Gifts* and save in the following location:

```text
S:\Development\Applications\Classy\Gift Exports\Classy Gift Exports FYXX-XX\Current Month
```

??? danger "Selecting the correct Classy transaction date range"

    It is essential to select the correct transaction date range when exporting Classy gifts to prevent duplicate and missing gifts. First, it's important to know that the **transaction date range is inclusive**. For example, a selected date range of 10/01/24 - 10/05/24 includes gifts from 10/01 and 10/05 in the exported report. Second, **DO NOT** ever select the current day (today's date) as the end date of the report. This may lead to missing gifts (gifts submitted on the same day but after you have exported the report) or duplicate gifts, as another gift entry team member may include the same date in a future export.

    To select the correct transaction date range, navigate to the Gift Exports folder listed above and find the most recent Classy export. Your **transaction start date** should be one day after the end date of the previous export. Your **transaction end date** should be at most the day before today's date. **However, there is no requirement for the how long a report has to be, but a report does need to be at least two days long (such as 10/01/24 - 10/02/24).** During a busy giving season, it is advantageous to use smaller date ranges to avoid fatigue during the gift entry process for Classy batches.

#### Preparing the Data
