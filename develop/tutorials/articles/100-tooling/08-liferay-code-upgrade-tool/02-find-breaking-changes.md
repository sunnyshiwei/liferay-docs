#LIFERAY CODE UPGRADE TOOL
#FIND BREAKING CHANGES 
###What are the Breaking Changes for Liferay 7.0?

In this tutorial, this document will presents a list of changes that break existing functionality,APIs,or contracts with third party Liferay developers or users.We try our best to minimize these discriptions, but sometimes they are unavoidable.

Here are some of types of changes documented in this file:

- Functionality that is removed or replaced
- API incompatibilities: Changes to public Java or JavaScript APIs
- Changes to context variables available to templates
- Changes in CSS classes available to Liferay themes and portlets
- Configuration changes: Changes in configuration files, like `portal.properties`, `system.properties`, etc.
- Execution requirements: Java version, J2EE Version, browser versions, etc.
- Deprecations or end of support: For example, warning that a certain feature or API will be dropped in an upcoming version.
- Recommendations: For example, recommending using a newly introduced API that replaces an old API, in spite of the old API being kept in Liferay Portal for backwards compatibility.

This function will help you to find breaking changes for type of java,jsp,xml and properties files.It will not support to find the front-end codes(eg.,javasripts,css).When you switch to the find breaking changes page.In addition to the descriptions,there will showing blank by default.And there are six button at the right of the view.

![Figure 1: Switch to Find Breaking Changes pages,showing blank by default.](/images/find-breaking-changes-first-page.png)

- **Find Breaking Changes:** help you to find the problems.
- **Automatically Correct Problems:** allow you to automatically correct the problems.
- **Expand All:** allow you to expand the project tree.
- **Collapse All:** allow you to collapse the project name.
- **Open Ignored List:** allow you to check or remove some ingnored problems.
- **Hide Tree:** hide all the tree and display the guidelines only.

###How to resolve breaking changes problems in Liferay Code Upgrade Tool? 

1.Click on the **Find Breaking changes** button.The *Project Selection* window will popup,you can select or deselect project,then click on **OK** button.

![Figure 2: When selecting *Find Breaking Changes* &rarr; *Select or Deselect* &rarr; *OK*, all the problems will be found.](/images/find-breaking-changes-button.png)

2.After find breaking changes,there will display the project tree at the top left.Expand all the project and click on one java or jsp file.You can see the problems and their guidelines in this page.

![Figure 3: You can fix problems according to the guidelins.](/images/find-breaking-changes-problems-page.png)

You can resolve the problems according to the guidelines.Here are the breaking changes guidelines main contents:

- **Date:** Specify the date you submitted the change. Format the date as YYYY-MMM (e.g., 2014-Mar) or YYYY-MMM-DD (e.g., 2014-Feb-25).
- **JIRA Ticket:** Reference the related JIRA ticket (e.g., LPS-123456) (Optional).
- **What changed?:** Identify the affected component and the type of change that was made.
- **Who is affected?:** Are end-users affected? Are developers affected? If the only affected people are those using a certain feature or API, say so.
- **How should I update my code?:** Explain any client code changes required.
Why was this change made? Explain the reason for the change. If applicable, justify why the breaking change was made instead of following a deprecation process.

(1) In the problem view,there are three column as below:

- **Resolved:** You can markdown the problem as resolved.
- **Line:** Display the line number,you can click on the *Line* to auto arrange the line as ascending and descending order.
- **Problem:** Display the problem title.

you can right click one problems check if it allow you to *Correct automatically*.You can correct this problems automatically,besides,all the allowed correct automatically problems can be resolved concurrently by click on the button **Automatically Correct Problems**.Then,you will find that all the allowed auto correct problems shouldn't be found.

Here are the five options when you right click one problem:

- **Mark done:** Make the checkbox *Resolved* of the problem as selected.but it's not resolved actually.
- **Mark undone:** Unselected the checkbox *Resolved*;
- **Ignore:** Ignore the selected problems.
- **Correct automatically:** Correct automatically the selected problems.
- **Ignore all problems of this type:** Ignore all problems of this type of the selected prolems.

![Figure 4: Right click on the problem,you are give five options for this problem.](/images/correct-automatically.png)

(2) Double click on one problem to open it,it will switch to the corresponding line number and showing the markdowns here.When you resolved this problem,the markdown and the red fork will disappear.

![Figure 5: If the problem resolved ,the markdown and red fork will disappear.](/images/markdown.png)

(3) Right click on the problem and select the option *Ignore all problems of this type*, all the same type of this problems will be ignored.You can go to **Open Ignored List** to check the ignored details.If you want to remove the ignored problems,you can *Select the problems* &rarr;*Remove* &rarr; *Apply* &rarr; *OK*.Now the ignored problems will be removed from the list.Then ,you can go to **Find Breaking Changes** to refind the problems.You will find that all the ignored problems will be find again.

![Figure 6: The removed problems details include *Tickets*,*Problem*,*Detail Information*.](/images/ignore-list-details.png)

(4) After you correct the problems Automatically,you need to resolve the rest of problems manually according to the guidelines.When you resolved them completely and didn't meet any issues.Congratulations,you made it.