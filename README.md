# Azure Immersion Workshop - Infrastructure Migration
## Hands on Labs Tips and Hints
A collection of tips and hints for use in Azure Immersion Workshop hands on labs delivered by Telstra Purple.

The Azure Immersion workshops are a collection of specific workshops dealing with different aspects of the cloud. See [here](https://partner.microsoft.com/en-US/solutions/azure/aiw) for a complete list. These workshops are delivered by trusted partners like Telstra Purple to customers.

This repository is simply a series of tips and tricks for those participating in the hands on labs component, where some confusion or difficulties may arise.

### Hands on Labs Tips

#### General
- When copy/pasting in the VM window, sometimes need to hit CTRL-C twice otherwise it retains only the previous copied item
	
#### Exercise 1 - Task 3 - Step 5
- Setting up Azure Migrate - appliance configuration manager - connection to Azure fails
  - Also popped up a dialog saying updates need to be installed (windows updates)
    - I selected to install updates
    - Wants to reboot VM - I rebooted
    - Once VM updates are installed - the connection to Azure works as expected.
	- Had a time when some updates failed and had to retry. The check for updates never quite completed but, the check Azure connection associated steps completed ok regardless.

#### Exercise 1- Task3 - Step 15
- The VM restarted for whatever reason so had to login to VM jumpbox, then back into Migrate assistant VM and it restarted the Migrate assistant process which means it checks connectivity to azure, syncs time, and check latest appliance updates which takes time
- This also takes you back to step 9

#### Exercise 1 - Task 5 - Step 8  --- Not clear how to get back there
- Return to dependencies
- Go to Azure Migrate - Servers-WebApps --> Groups -> SMartHotelVM's --> SmartHotelWeb1 link for Requires User agent
- Also, when right clicking links and copy/pasting to notepad, had to right click and select copy link TWICE otherwise it would retain the old link value not the one you wanted
	
#### Exercise 1 - Task 5 - Step 28
- Once sudo elevated into UbuntuVM - cannot copy/paste wget command!!
- However, 
  - Click on top left of cmd window - select edit -> paste then
  - right click into session pastes the command
  - Or ctrl-V, then mouse right click


#### Exercise 2 - Task 3 - Database Schema Migration
- Had an issue where I performed a schema migration which completed successfully. However the lab validation fails onm this step.
  - Have lodged a support email to verify whether I have missed something or its a bug
- Addtionally, the data migration reported as still running on the main blade even though the process itself completed.
- Update: After a while the data migration shows completed on the main blade **and** the lab now validates.
<img width="636" alt="image" src="https://user-images.githubusercontent.com/435165/193194975-2c296820-1cfd-4997-9dcd-9aee171737d2.png">
