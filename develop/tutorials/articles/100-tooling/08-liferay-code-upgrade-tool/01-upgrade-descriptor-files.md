#LIFERAY CODE UPGRADE TOOL

#UPGRADE DESCRIPTOR FILES 

In this tutorial, you'll learn how to upgrade descriptor xml dtd version from 6.2 to 7.0 and delete wap-template-path tag in liferay-layout-template.xml.When you switch to the upgrade descriptor files page you will find that all the xml files which need to upgrade will display by default.

But when you restart the liferay code upgrade tool view,you should clicking on **Find** button to display the files which need to upgrade.

![Figure 1: This page displaying all the files which need to upgrade.](/images/showing-all-the-files.png)

 Double click the file in the list.It will popup a comparison page which shows the differences between your original source file and upgrade preview file.

![Figure 2: The shaded area showing the differences of Source file and Upgrade file.](/images/comparison-page.png)

Now you can check all the files by clicking on these files in the list.Click **Upgrade** button, the files will upgrading to 7.0 version.Double click the upgraded file in the list,the source file are the same as the upgrade file.And all the color of the upgraded files name will change to blue.

![Figure 3: The upgraded files name turned to blue.](/images/upgraded-file-color.png)

Click **Find** button again.All the upgraded files will disappear because the files have been upgraded.And there will showing the warning message as below:

![Figure 4: The files have already upgrade.](/images/wraning-message1.png)

Click **Upgrade** button again.There will showing the wraning message as below because there are no files need to upgrade:

![Figure 5: There are no files need to upgrade.](/images/wraning-message2.png)

At the bottom of the liferay code upgrade tool view,there are four symbols that in oder to prompting users to get the status of these functions.


`← button:` will help you return pervious page.

`√ button:` will help you mark which page that you have finished.

`× button:` will help you mark which page that you haven't finished.

`→ button:` will help you go to next page.

