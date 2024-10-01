# Identity and Access Management(IAM)
- A way to granting access to AWS resources.
- Access key ID and secret access keys are not the same as username and passwords.
	- Always set up password rotation policies.
	- You only get to view these once -> If you lose them, you have to regenerate them. So, save them in a secure location. 
- Allows you to manage users and their level of access to the AWS console.
	- Create users and grant permissions to those users.
	- Create groups and roles.
	- Control access to AWS resources.
- **Root account**: Is the email address you used to sign up for AWS. The root account has **full administrative access to AWS**. For this reason, it's important to secure this account.
	- Add MFA to the root account.
	- Create an admin group for your administrators, and assign the appropiate permissions to this group.
	- Create user accounts for your administrators.
	- Add your users to the admin group.

- **Users**: Physical person. 
	- New users: No permissions when first created.
	- Always work on the principle that one user equals one physical person.
	- Never share user accounts across multiple people.
	- **Principle of Least Privilege**: Only assign a user the minimum amount of privileges they need to do their job.
- **Groups**: Functions, such as administrator, developer, etc -> Contains users.
	- It's best practice for users to inherit permissions from groups.
- **Roles**: Internal usage with AWS -> Allows one part of AWS to access another part of AWS.

- IAM Federation: You can combine your existing user account with AWS. For example, when you log on to your PC, you can use the same credentials to log in to AWS if you set up federation.
- Identity Federation: Uses the SAML standard, which is Active Directory.