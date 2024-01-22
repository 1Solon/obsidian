* An **IAM user** is a person or application that is defined in an AWS account, and that must make API calls to AWS products. Each user must have a unique name (with no spaces in the name) within the AWS account, and a set of security credentials that is not shared with other users. These credentials are different from the AWS account root user security credentials. Each user is defined in one and only one AWS account.

**IAM User Authentication:**
![[Pasted image 20210927094133.png]]
* This follows the basic definition of [[Authentication]]
* If you grant programmatic access, the IAM user will be required to present anaccess key IDanda secret access keywhen they make an AWS API call by using the AWS CLI, the AWS SDK, or some other development tool.
* If you grant AWS Management Console access, the IAM user will be required to fill in the fields that appear in the browser login window. The user is prompted to provide either the 12-digit account ID or the corresponding account alias. The user must also enter their IAM user name and password. If multi-factor authentication (MFA) is enabled for the user, they will also be prompted for an authentication code.
