# Deploying your Python script to the cloud with Azure for Students

**Meet Megan.**

<img src="images/megandoc.png" width="200">

Megan is a junior in college. She's taking a Python course and working on her final project. Like many college students, Megan couldn't afford a powerful laptop. When she tried to run her final project on her computer, she realized that it would take weeks for the program to finish running. She didn't have weeks to wait. She needed a solution. But what?

**Megan, meet Azure for Students.**

With a free Azure for Students account, you can deploy your Python scripts to a powerful virtual machine and cut your run-time significantly. Azure for Students gives students $100 in free credits every year.

You're charged by the minute, so it's important to use your virtual machine only when you need it, and turn it off immediately when you're done. Whatever remaining credits you have can then be used within a year of your sign-up date.

Are you in a situation similar to Megan’s? Azure for Students is for you, too. Let me show you how to get started!

## Download Remote Desktop Protocol Client

Before you start, download [Remote Desktop Protocol Client](https://docs.microsoft.com/en-us/windows-server/remote/remote-desktop-services/clients/remote-desktop-clients) (RDP client) and follow the applicable link for your computer. RDP client allows you to control other computers remotely, which is how you will use your virtual machine.

## Sign up for Azure for Students 
1. Go to [Azure for Students](https://azure.microsoft.com/en-us/free/students/).
2. Select **Activate now** and log in with school email.
3. Follow prompts to create Azure for Students account.

## Deploy virtual machine
1. On [Azure Portal](https://portal.azure.com), search "virtual machine".
2. Select **Add** > **Virtual machine**.
3. Create virtual machine.
<ol>
<ul>
<ol type="a">
  <li>Name your virtual machine.</li>
  <li>Pick region to deploy.</li>
      <b>Tip:</b> Pick region physically closest to you for quickest connection.
  <li>For image, select <b>Windows 10 Pro, Version 1809 - Gen 1</b>.</li>
  <li>For size, select <b>Standard_D4S_v3</b>.</li>
      <b>Note:</b> You may need to select <b>See all sizes</b> to find this option.
  <li>Create administrator account for virtual machine by setting username and password.</li>
  <li>Leave rest as default and confirm licensing.</li>
  <li>Select <b>Review + create</b>.</li>
      <b>Note:</b> When the validation passes, select <b>Create</b> to deploy your virtual machine.
</ol>
</ol>

## Connect to virtual machine
1. When deployment completes, select **Go to resource**.
2. Find Public IP address and copy it.
3. Open RDP client and select **Add PC**.
4. Under PC name, pasted copied IP address.
5. Assign friendly name and select **Add**.<br />
**Note:** Virtual machine will appear on RDP client screen.
6. Connect to virtual machine and enter administrator account username and password.
7. Select **Continue**.<br />
**Note:** You will redirect to your virtual machine.

## Install Python on virtual machine
On virtual machine, download latest version of Python from [Microsoft Store](https://www.microsoft.com/en-us/search?q=python).

## Move files to virtual machine
Copy and paste your Python file from normal desktop to virtual machine desktop.

## Run script on virtual machine
1. On virtual machine, open a command prompt.
2. Run your Python script.

## Stop virtual machine
When done running your script, stop your virtual machine to stop being charged.
1. On [Azure Portal](https://portal.azure.com), select your virtual machine.
2. Select **stop** > **OK**.

