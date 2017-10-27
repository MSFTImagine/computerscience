This folder contains scripts that complement the functionality of the Azure Education portal
<table>
<tr>
<td>Task</td>   <td>Script</td>   <td> Documentation </td>
</tr>
<tr>
<td>Bulk Sandbox Deployment Automation</td>
<td>change-vm-state.sh</p>create-vm-image.sh</p> deploy-vm.sh</td>
<td>Educators want a simple way to provide students with VMs based on a specific VM image (for example, Data Science VM), so students can learn the fundamentals of data science. These scripts achieve the following user stories:</p>
Ability to deploy multiple DSVMs (Data Science Virtual Machine) in either Windows, Ubuntu, of Linux CentOS</p>
Ability to deploy VMs from marketplace image, custom image, or DSVM</p>
Ability to deploy VMs across one or multiple subscriptions (i.e. Each VM can be in its own subscription)</p>
Ability for each VM to have its own Resource Group</p>
Ability to create a clean VM image from a VM</td>
</tr>
<td>Create bulk accounts </td>
<td>createstudents.sh and Students.csv</td>
<td>This bash script will read a list of accounts to create from a csv to bulk create email adresses for students taking a course. It will assign an Azure subscription to each of the students.
Full instructions can be found in the file createstudentsInstructions.md  
IMPORTANT NOTE:   
**Accounts created with this script will NOT be able to access the [Azure classic portal](https://manage.windowsazure.com)**   
This script creates accounts based on Role Based Access Control (RBAC) and puts limitations on the accounts created. You can see a complete list of features available in 
the Azure portal vs the Azure classic portal in this <a href="https://azure.microsoft.com/en-us/features/azure-portal/availability/">Azure portal availability chart</a> 

</td>
<tr>
<td> View billing information </td>
<td> <a href="https://github.com/Microsoft/AzureUsageAndBillingPortal">Azure Billing Portal</a> </td>
<td> Viewing detailed account usage presents challenges when using credit based subscriptions. The Azure Usage and billing portal is a complete solution that creates
a website and PowerBI dashboard to visualize Azure service billing and usage details.  This solution can be used whether students are given access to Azure through the Azure Education 
Portal subscriptions or through Azure passes. You set up the solution for the faculty member. The students register their Azure subscription wih the system and the professor is able to
view usage and billing for each registered user. Full documentation on how to install and use the tool is available on Github <a href="https://github.com/Microsoft/AzureUsageAndBillingPortal">Azure Billing Portal GitHub</a>
</tr>
</td>
<tr>
<td> Powershell Function for creating Azure Resource Groups and signing user access perfect solution for Group projects</td>
<td> EduPortalAzureBulkCreate.psm1 NewUsers.csv and NewResourceGroups.csv</td>
<td> This is a set of powershell script which will help you perform tasks on your azure subscriptions. 
Simply run the command functions within poweshell  -  Functions - function New-Users - Creates new users based on content of the CSV - function New-ResourceGroups - Creates new resource group and add users based on 
CSV content Function - function Set-RBACPermissions - creates role based access control permission based on CSV
</tr>

</td>
<tr>
<td> Bulk Adding AAD Existing users via Powershell</td>
<td> BulkAddAAD.ps1 and Data.txt</td>
<td> This powershell script will read a list of accounts to a .txt file It will assign an Azure subscription to each of the students.
Full instructions can be found in the file BulkAddAADInstructions.md  
IMPORTANT NOTE:   
**Accounts created with this script will NOT be able to access the [Azure classic portal](https://manage.windowsazure.com)**   
This script creates accounts based on Role Based Access Control (RBAC) and puts limitations on the accounts created to a contributor. You can see a complete list of features available in 
the Azure portal vs the Azure classic portal in this <a href="https://azure.microsoft.com/en-us/features/azure-portal/availability/">Azure portal availability chart</a></tr>
</tr>

</td>
<tr>
<td> Listing all your Azure Subscription via Powershell</td>
<td> ListAzureSubs.ps1 </td>
<td> This powershell script will list of the Azure Subscriptions and then list a table format of the Azure SubscriptionName and Azure SubscriptionID. 
Simply run the command Navigate to the directory where the script lives 
PS> cd C:\my_path\yada_yada\ (enter) 
Execute the script: PS> .\ListAzureSubs.ps1 (enter)
Or: you can run the PowerShell script from cmd.exe like this:
powershell -noexit C:\my_path\yada_yada\ListAzureSubs.ps1 (enter)
Simply then copy and paste your Subscription IDs into the Excel for assigning users
</tr>

</td>
<tr>
<td> Useful Comamds Azure Subscription via Powershell</td>
<td> AzureSubsCommands.md </td>
<td> This is a set of powershell script which will help you perform tasks on your azure subscriptions. 
Simply run the command within poweshell 
</tr>

</table>
