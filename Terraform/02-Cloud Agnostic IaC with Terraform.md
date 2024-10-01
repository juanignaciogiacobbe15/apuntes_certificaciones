# Terraform
- Automate Software Defined Networking.
- Interacts and takes care of communication with control layer APIs with ease.
- Supports a vast array of private and public cloud vendors.
- Tracks state of each resource deployed.
- Executes code in files with the `.tf` extension.

![](img/Pasted%20image%2020240918110451.png)


## Initializing the Working Directory

- Initializes the working directory that contains your Terraform Code
	- Downloads ancillary components(modules and plugins).
	- Sets up the backend for storing Terraform state file, a mechanism by which Terraform tracks resources.
```
terraform init
```


- Reads the code and then creates and shows a "plan" of execution/deployment. It doesn't deploy anything(consider a read-only command).
- Allows the user to "review" the action plan before executing anything.
- At this stage, authentication credentials are used to connect to your infrastructure, if required.
```
terraform plan
```


- Deploys the instructions and statements in the code.
- Updates the deployment state tracking mechanism file, a.k.a. "state file".
```
terraform apply
```


- Looks at the recorded, stored state file created during deployment and destroys all resources created by your code.
- Should be used with caution, as it is a non-reversible command. Take backups, and be sure that you want to delete infrastructure.
```
terraform destroy
```


## Configuring the Provider

![](../Pasted%20image%2020240918113217.png)


![](../Pasted%20image%2020240918113302.png)

![](../Pasted%20image%2020240918113523.png)