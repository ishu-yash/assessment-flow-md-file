## Levelops: Triage Flow
 On clicking **Triage** option from the sidebar user is navigated to [http://localhost:3000/#/admin/triage](http://localhost:3000/#/admin/triage). Here user is presented with three tabs namely:
 - [**Triage Results**](#triage-results)
 - [**Triage Rules**](#triage-rules)
 - [**Triage Grid View**](#triage-grid-view)
 ## <a id="triage-results">Triage Results :</a>
 - This is the default active tab.
 - The **Triage Result Table**  consists of five columns:
   - **Name :**  
	   - On clicking any cell user is navigated to [http://localhost:3000/#/admin/triage/view?id={id}](http://localhost:3000/#/admin/triage/view).  Here **id** is the id of the clicked triage result.
	   - On the **Triage View** page user can **View Logs** of the selected triage result and gets the integral details about the selected triage result.
	   
	   - User can filter the **Stages/Jobs** on the basis of result and state using **Filters** provided.
	- **Run Number**
	- **Updated On**
	- **Result**
	- **CI/CD User**
- User can search specific triage results by typing keywords on the search handler provided.

- User can filter triage results on the basis of **Name**, **Status**, **CI/CD User** and **Date Between**.

 ## <a id="triage-rules">Triage Rules :</a>
- On clicking **Triage Rules** tab, user is navigated to [http://localhost:3000/#/admin/triage?tab=triage_rules](http://localhost:3000/#/admin/triage?tab=triage_rules).

 - The **Triage Rules Table**  consists of three columns:
   - **Name :** 
	   - On clicking any cell user is navigated to [http://localhost:3000/#/admin/triage/rules/edit?rule={id}](http://localhost:3000/#/admin/triage/rules/edit) Here **id** is the id of the clicked  triage rule.
	   - On **Triage Rule Edit Page** user can set/change **Name**, **Description**, **Owner**, **Application** and also can add **Regexes**.
	   
	   - Once user has finished editing, clicking on **Save** button takes user back to [http://localhost:3000/#/admin/triage?tab=triage_rules](http://localhost:3000/#/admin/triage?tab=triage_rules).
   - **Updated On :** This gives info about last updation of triage rule in the form of date.
  
   - **Actions :** There is a **Delete** action button, clicking which opens a popover which asks for confirmation of deletion. Once user clicks on **Ok** button the triage rule gets deleted.
- User can search specific triage rule by typing keywords on the search handler provided.
## <a id="triage-grid-view">Triage Grid View :</a>
- On clicking **Triage Grid View** tab, user is navigated to [http://localhost:3000/#/admin/triage?tab=triage_grid_view](http://localhost:3000/#/admin/triage?tab=triage_grid_view).
- On this page, there are two grids:
	- First grid shows list of **Triage Results** along with daily status in terms of number of **Success**, **Failed** and **Aborted**. 
		- Clicking on the **Name** of the **Triage Result**  will navigate to [http://localhost:3000/#/admin/triage?job_names={job-name}&tab={tab-id}](http://localhost:3000/#/admin/triage?job_names=%7Bjob-name%7D&tab=%7Btab-id%7D). Here **job-name** is the **Triage Result Name** and **tab-id** is the tab name of the respective tab.
		
		- Clicking on **i** icon ( adjacent to number) on the grid opens a **Issue Drawer** which shows a list of **issues** along with the respective **assignees** and **status**.
		- Clicking on any issue from the list, the user is navigated to [http://localhost:3000/#/admin/workitems/details?workitem={id}](http://localhost:3000/#/admin/workitems/details?workitem=%7Bid%7D). Here **id** is the id of clicked issue. Here user can create/edit the issue.
	- Second grid is about **Daily Totals** of **Success**, **Failure** and **Aborted**.
- User can download the **Triage Grid** in **CSV** format by clicking on **Download as CSV** button.

- User can filter the grid data  on the basis of **Name**, **Parent Job Name**, **Status**, **Date Between** and **Triage Rules**. 
 ## Similar To All Flow :
 At the top right corner, user has a button with name :
 - **Add Triage Rule :** 
	 - On Clicking this button user is navigated to [http://localhost:3000/#/admin/triage/rules/create](http://localhost:3000/#/admin/triage/rules/create) .
	 
	 - On **Triage Rule Create** page user can set/change **Name**, **Description**, **Owner**, **Application** and also can add **Regexes**. 
	 - After filling all the required fields user can click on **Save** button which creates new triage rule and user gets navigated to [http://localhost:3000/#/admin/triage?tab=triage_rules](http://localhost:3000/#/admin/triage?tab=triage_rules).
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTQ0OTUwNTM3OF19
-->