**Step 1:**
![[Pasted image 20210927111110.png]]

**Step 2:**
![[Pasted image 20210927111147.png]]

* Another recommended step for securing a new AWS account is to require multi-factor authentication (MFA) for the account root user login and for all other IAM user logins. You can also use MFA to control programmatic access

* You have a few options for retrieving the MFA token that is needed to log in when MFA is enabled. Options include virtual MFA-compliant applications (such as Google Authenticator and Authy Authenticator), U2F security key devices, and hardware MFA options that provide a key fob or display card.

**Step 3:**
![[Pasted image 20210927111258.png]]

* Enable [[AWS Cloudtrail]]

**Step 4:**
![[Pasted image 20210927111630.png]]

* An additional recommended step for securing a new AWS account is to enable billing reports, such as the AWS Cost and Usage Report. Billing reports provide information about your use of AWS resources and estimated costs for that use. AWS delivers the reports to an Amazon S3 bucket that you specify and AWS updates the reports at least once per day. 

* The AWS Cost and Usage Report tracks usage in the AWS account and provides estimated charges, either by the hour or by the day.
