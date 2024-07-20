

Active Directory User Termination Script

This PowerShell script automates the process of terminating a user’s account in Active Directory. It performs the following actions:

Clears the Manager Attribute: The script removes the manager attribute from the user’s account.

Disables the User Account: The script checks if the user account exists and is enabled. If so, it prompts for confirmation before disabling the account.

Removes Group Memberships: The script removes the user from all groups they are a member of.

Moves the User Account: The script moves the user account to the Desired Organizational Unit (OU).

The script prompts for the full name and username of the account to disable. It then calls the Disable-UserAccount function, which performs the above actions. The script continues to prompt for user accounts to disable until the user chooses to stop.




Usage

Run the script in a PowerShell environment. When prompted, enter the full name and username of the account you wish to disable.

Requirements

The script requires the Active Directory PowerShell module.
The user running the script needs the necessary permissions to disable accounts in Active Directory.

Disclaimer

Please use this script with caution. Always confirm the details of the account before disabling it. It’s recommended to test this script on a small number of accounts first to ensure everything is working as expected.
