# Managing an AWS Account<a name="manage-account-payment"></a>

You can use the Billing and Cost Management console to change account settings, including your contact and alternate contact information, the currency that you pay your bills in, the Regions that you can create resources in, and your tax registration numbers\.

**Note**  
Some sections can only be edited by the AWS account root user\. If you do not see the **Edit** option, switch to the root user\.

**Topics**
+ [Editing Your User Name, Password, and Email Address](#manage-account-payment-edit-user-name)
+ [Editing Contact Information](#manage-account-payment-edit-contacts)
+ [Changing Which Currency You Use to Pay Your Bill](#manage-account-payment-change-currency)
+ [Adding, Changing, or Removing Alternate Contacts](#manage-account-payment-alternate-contacts)
+ [Enabling and Disabling Regions](#manage-account-payment-enable-disable-regions)
+ [Updating and Deleting Tax Registration Numbers](#manage-account-payment-update-delete-tax-numbers)

## Editing Your User Name, Password, and Email Address<a name="manage-account-payment-edit-user-name"></a>

To edit your user name, password, or email address, perform the following procedure\.<a name="account-info"></a>

**To edit your user name, password, or email address**

You can change the name, password, and email address associated with your account\.

1. Sign in to the AWS Management Console and open the Billing and Cost Management console at [https://console\.aws\.amazon\.com/billing/home\#/](https://console.aws.amazon.com/billing/home)\.

1. On the navigation bar, choose your account name, and then choose [https://console.aws.amazon.com/billing/home#/account](https://console.aws.amazon.com/billing/home#/account)\.

1. On the **Account Settings** page, next to **Account Settings**, choose **Edit**\.

1. Next to the field to update, choose **Edit**\.

1. After you have entered your changes, choose **Save changes**\.

1. After you have made all of your changes, choose **Done**\.

## Editing Contact Information<a name="manage-account-payment-edit-contacts"></a>

You can change the contact information associated with your account, including your mailing address, telephone number, and website address\. To edit your contact information, perform the following procedure\.<a name="contact-info"></a>

**To edit your contact information**

1. Sign in to the AWS Management Console and open the Billing and Cost Management console at [https://console\.aws\.amazon\.com/billing/home\#/](https://console.aws.amazon.com/billing/home)\.

1. On the navigation bar, choose your account name, and then choose [https://console.aws.amazon.com/billing/home#/account](https://console.aws.amazon.com/billing/home#/account)\.

1. Under **Contact Information**, choose **Edit**\.

1. For the fields to change, enter your updated information and then choose **Update**\.

**Note**  
You can add an email address for billing in the **Alternate Contacts** section to have AWS send a copy of billing\-related emails to that email address\. For example, AWS sends your **Billing contact address** a message that your monthly bill is ready\.

## Changing Which Currency You Use to Pay Your Bill<a name="manage-account-payment-change-currency"></a>

To change the currency that you use to pay your bill, for example, from Danish kroner to South African rand, perform the following procedure\.<a name="local-currency"></a>

**To change the local currency associated with your account**

1. Sign in to the AWS Management Console and open the Billing and Cost Management console at [https://console\.aws\.amazon\.com/billing/home\#/](https://console.aws.amazon.com/billing/home)\.

1. On the navigation bar, choose your account name, and then choose [https://console.aws.amazon.com/billing/home#/account](https://console.aws.amazon.com/billing/home#/account)\.

1. Scroll down to the **Payment Currency Preference** section\. Next to **Payment Currency Preference**, choose **Edit**\.

1. For **Select Payment Currency**, select the currency to pay your bill in and then choose **Update**\.

## Adding, Changing, or Removing Alternate Contacts<a name="manage-account-payment-alternate-contacts"></a>

Alternate contacts enable AWS to contact another person about issues with your account, even if you're unavailable\. To add, change, or delete alternate contacts for your account, perform the following procedure\.<a name="account-contacts"></a>

**To add, update, or remove alternate contacts**

1. Sign in to the AWS Management Console and open the Billing and Cost Management console at [https://console\.aws\.amazon\.com/billing/home\#/](https://console.aws.amazon.com/billing/home)\.

1. On the navigation bar, choose your account name, and then choose [https://console.aws.amazon.com/billing/home#/account](https://console.aws.amazon.com/billing/home#/account)\.

1. Scroll down to the **Alternate Contacts** section and choose **Edit**\.

1. For the fields to change, enter your updated information and choose **Update**\.

## Enabling and Disabling Regions<a name="manage-account-payment-enable-disable-regions"></a>

AWS originally enabled all new Regions by default, which enabled your users to create resources in any Region\. Now when AWS adds a Region, the new Region is disabled by default\. If you want your users to be able to create resources in a new Region, you enable the Region\.

Note the following about enabling and disabling Regions:

**You can use IAM permissions to control access to Regions**  
IAM added three new permissions, which let you control which users can enable, disable, and list Regions\. For more information, see [Billing Actions](billing-permissions-ref.md#user-permissions)\.

**Enabling a Region is free**  
There is no charge to enable a Region\. You're only charged for resources that you create in the new Region\.

**Disabling a Region disables access to resources in the Region**  
If you disable a Region that still includes AWS resources, such as Amazon EC2 instances, you can't access the resources in that Region\. For example, you can't use the AWS Management Console or any programmatic method to view or change the configuration of any EC2 instances in that Region\.

**Charges continue if you disable a Region**  
If you disable a Region that still includes AWS resources, charges for those resources \(if any\) continue to accrue at the standard rate\. For example, if you disable a Region that contains Amazon EC2 instances, you still have to pay the charges for those instances even though the instances are inaccessible\.

**Disabling a Region isn't always immediately visible**  
If you disable a Region, the change takes time to become visible in all possible endpoints\. Disabling a Region can take between a few seconds to minutes to take effect\. 

**Existing Regions are enabled by default**  
The original Regions \(the Regions that existed before we added the ability to enable and disable Regions\) are all enabled by default and can't be disabled\.

**Enabling a Region takes a few minutes for most accounts**  
Enabling a Region generally takes effect in a few minutes, although it can take longer for some accounts\. If enabling a Region takes longer than nine hours, sign in to the AWS Support Center and open a case with AWS Support\.

Perform the applicable procedure:
+ [To enable a Region](#enable-region)
+ [To disable a Region](#disable-region)<a name="enable-region"></a>

**To enable a Region**

1. Sign in to the AWS Management Console and open the Billing and Cost Management console at [https://console\.aws\.amazon\.com/billing/home\#/](https://console.aws.amazon.com/billing/home)\.

1. On the navigation bar, choose your account name, and then choose [https://console.aws.amazon.com/billing/home#/account](https://console.aws.amazon.com/billing/home#/account)\.

1. Under **AWS Regions**, next to the Region to enable, choose **Enable**\.

   Older Regions are enabled by default\.

1. In the dialog box, choose **Enable region**\.

For more information about enabling a Region, including the permissions required, see [Managing AWS Regions](https://docs.aws.amazon.com/general/latest/gr/rande-manage.html)\.<a name="disable-region"></a>

**To disable a Region**

You can disable some Regions on your **My Account** page\.

1. Sign in to the AWS Management Console and open the Billing and Cost Management console at [https://console\.aws\.amazon\.com/billing/home\#/](https://console.aws.amazon.com/billing/home)\.

1. On the navigation bar, choose your account name, and then choose [https://console.aws.amazon.com/billing/home#/account](https://console.aws.amazon.com/billing/home#/account)\.

1. Under **AWS Regions**, next to the Region to disable, choose **Disable**\.

   Not all Regions can be disabled\.

1. In the dialog box, for **To confirm disabling in this region, ** enter **disable** and choose **Disable region**\.

## Updating and Deleting Tax Registration Numbers<a name="manage-account-payment-update-delete-tax-numbers"></a>

To update or delete one or more tax registration numbers, perform the applicable procedure:
+ [To update tax registration numbers](#edit-tax)
+ [To delete tax registration numbers](#remove-tax)<a name="edit-tax"></a>

**To update tax registration numbers**

1. Sign in to the AWS Management Console and open the Billing and Cost Management console at [https://console\.aws\.amazon\.com/billing/home\#/](https://console.aws.amazon.com/billing/home)\.

1. In the navigation pane, choose **Tax Settings**\.

1. Under **Manage Tax Registration Numbers**, select the numbers to edit\.

1. For **Manage Tax Registration**, choose **Edit**\.

1. Update the fields to change and choose **Update**\.<a name="remove-tax"></a>

**To delete tax registration numbers**

You can remove one or more tax registration numbers\. 

1. Sign in to the AWS Management Console and open the Billing and Cost Management console at [https://console\.aws\.amazon\.com/billing/home\#/](https://console.aws.amazon.com/billing/home)\.

1. In the navigation pane, choose **Tax Settings**\.

1. Under **Manage Tax Registration Numbers**, select the tax registration numbers to delete\.

1. For **Manage Tax Registration**, choose **Delete**\.

1. In the **Delete tax registration** dialog box, choose **Delete**\.