<a href="https://www.youtube.com/watch?v=PoMPOGvctzs&ab_channel=SalesforceOutOfTheBox">
  <img src="https://raw.githubusercontent.com/afawcett/githubsfdeploy/master/src/main/webapp/resources/img/deploy.png" alt="Deploy to Salesforce" />
</a>

<a href="https://githubsfdeploy.herokuapp.com?owner=financialforcedev&amp;repo=apex-mdapi">
  <img src="https://media2.giphy.com/media/v1.Y2lkPTc5MGI3NjExMjk4ZTBjODM5M2FlYjcxYmQ0NTY3MmE1NzhhZjc2NGM3Y2VlYzk0OSZjdD1n/KF4QviO3H0JjBaLzVn/giphy.gif" />
</a>
# Salesforce DX Project: Next Steps

Now that you’ve created a Salesforce DX project, what’s next? Here are some documentation resources to get you started.

## How Do You Plan to Deploy Your Changes?

Do you want to deploy a set of changes, or create a self-contained application? Choose a [development model](https://developer.salesforce.com/tools/vscode/en/user-guide/development-models).

## Configure Your Salesforce DX Project

The `sfdx-project.json` file contains useful configuration information for your project. See [Salesforce DX Project Configuration](https://developer.salesforce.com/docs/atlas.en-us.sfdx_dev.meta/sfdx_dev/sfdx_dev_ws_config.htm) in the _Salesforce DX Developer Guide_ for details about this file.

## Read All About It

- [Salesforce Extensions Documentation](https://developer.salesforce.com/tools/vscode/)
- [Salesforce CLI Setup Guide](https://developer.salesforce.com/docs/atlas.en-us.sfdx_setup.meta/sfdx_setup/sfdx_setup_intro.htm)
- [Salesforce DX Developer Guide](https://developer.salesforce.com/docs/atlas.en-us.sfdx_dev.meta/sfdx_dev/sfdx_dev_intro.htm)
- [Salesforce CLI Command Reference](https://developer.salesforce.com/docs/atlas.en-us.sfdx_cli_reference.meta/sfdx_cli_reference/cli_reference.htm)


Use Case:
Universal Container(UC) is an Auto Manufacturing company that wants to show all the related Accounts and Contacts related to the Vehicle on the Vehicle detailed page for their service Advisors. The advisors should be able to create cases and manage users from the ARC layout. The Vehicle can have the following stakeholders. 

Current Owner
Previous Owner
Primary Driver
Secondary Driver
Referral Account Details
Selling Dealer
Servicing Dealer

Note: UC wants to deliver the above feature out of the box(OOTB).

Solution: 

We will use Salesforce Auto Cloud OOTB objects to implement the features. 
Use Assets and Vehicles to manage the current ownership.
Use Asset Account Participation object to showcase Previous Owner and Dealership details. 
Use Asset Contact Participation object to house Driver details. 
Use the Account Contact Relation object to capture the referral details. 
We can create a record type or Use the Salesforce OOTB Account Type field to segregate different customer types. In my example, I made two record types, Household and Dealer.

Note: I tried to make this example simple and tried to implement 100% OOTB configuration. 

