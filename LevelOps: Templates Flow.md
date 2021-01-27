# LevelOps: Templates Flow
* [Assessments Templates Flow](#assessment-templates)
* [Issue Template Flow](#issue-templates)
* [Similarities Between Two Flows](#common)

## <a id="assessment-templates">Assessments Templates Flow :</a>

 1. On clicking  **Assessments Templates** option, user is navigated to [http://localhost:3000/#/admin/templates/assessment-templates](http://localhost:3000/#/admin/templates/assessment-templates)
 2. Here user has two buttons at the top right corner namely:
     - **Import from CSV :**
         - On clicking this button a **Modal** opens up which offers, drag and drop or browse from device, for uploading CSV file.
     - **Add Assessment Template :**
         - On clicking this button user is navigated to [http://localhost:3000/#/admin/templates/assessment-templates/create](http://localhost:3000/#/admin/templates/assessment-templates/create) and a **Assessment Template Settings** modal opens up by default. This modal allows user to set  basic information about the template like **Name**, **Knowledge Base**, **Tags**  etc. 
         -  Clicking on cancel will redirect you back to [http://localhost:3000/#/admin/templates/assessment-templates](http://localhost:3000/#/admin/templates/assessment-templates)
         
         - On clicking **Ok** button a basic skeleton of users new assessment template is created.
         - Now user can edit the template by adding more sections. Each section can have any number of questions.
       
         - Once, user has added all the sections, user can save the assessment template by clicking **Save** button which navigates the user back to [http://localhost:3000/#/admin/templates/assessment-templates](http://localhost:3000/#/admin/templates/assessment-templates) or can edit assessment settings by clicking **Settings** button which opens **Assessment Template Settings** modal. 
 
 3. User is presented with a table which has following four columns:
    - **Name :**
	    - On clicking any cell user is navigated to [http://localhost:3000/#/admin/templates/assessment-templates/edit?questionnaire={id}](http://localhost:3000/#/admin/templates/assessment-templates/edit).  Here **id** is the id of clicked assessment template. 
	    - On the current open page, user can edit the template by adding more sections to it. Each section can have any number of questions.
	
         - Once, user has added all the sections, user can save the assessment template by clicking **Save** button which navigates the user back to [http://localhost:3000/#/admin/templates/assessment-templates](http://localhost:3000/#/admin/templates/assessment-templates) .
         - User can edit assessment settings by clicking **Settings** button  which opens **Assessment Template Settings** modal . This modal allows user to set  basic information about the template like **Name**, **Knowledge Base**, **Tags**  etc. 
         On clicking **Ok** button new settings are applied. 
		- User can also export the selected assessment template by clicking on **Export** button.
     - **Updated on :** This column gives date of template's last updation.
     - **Tags :** This column gives info about tags added to the assessment.
     - **Actions :** This column is provided with actions namely **Clone**, **Export** and **Delete** the assessment template.
 4. User can filter the assessment list on the basis of tags, by clicking on filter button which offers, user a list of tags to select from. On selecting tags, filters are applied to the list.
## <a id="issue-templates"> Issue Template Flow :</a>
 1. On clicking  **Issue Templates** option, user is navigated to [http://localhost:3000/#/admin/templates/issue-templates](http://localhost:3000/#/admin/templates/issue-templates).
 
 3. Here user has one button at top right corner :
	 - **Add Issue Template :**
	   -  On clicking this button user is navigated to [http://localhost:3000/#/admin/templates/issue-templates/edit](http://localhost:3000/#/admin/templates/issue-templates/edit) which is **Configure Template** page. 
	   - This page allows user to add custom metadata fields and assessments to the ticket template.
	   
	   - Here user can set/change settings of the issue templates by clicking **Settings** button at the top right corner. A **Settings Modal** opens with allows user to edit basic settings like **Name** and **Description** of the template etc. On clicking **Ok** button, settings are applied.
	 
		- Once user has set Template name in **Settings**, **Save** button is enabled and now user can save issue template. On clicking **Save** button user is navigated back to [http://localhost:3000/#/admin/templates/issue-templates](http://localhost:3000/#/admin/templates/issue-templates).
 4. User is presented with a table which has following five columns:
	- **Name :**	    
		- On clicking any cell user is navigated to [http://localhost:3000/#/admin/templates/issue-templates/edit?template={id}](http://localhost:3000/#/admin/templates/issue-templates/edit).  Here **id** is the id of clicked issue template. The function of the current page is same as the page to which user gets navigated on clicking **Add Issue Template** button.
	- **Updated On :** This column gives date of last updation of issue template.
	 - **Enabled :** This column tells whether the issue template is enabled or not.
	- **Default**: This column tells whether the issue template is default or not.
	- **Actions :** This column is provided with actions namely **Clone** and **Delete** for cloning  and deleting the issue template respectively.
## <a id="common">Similarities Between Two Flows :</a>
 1. **Cloning :** Assessment Template List and Issue Template List both are provided with an action button for cloning template. On clicking the clone button, a popover opens which asks for confirmation for cloning. On clicking **Ok** button, the selected template is cloned.
 
 2. **Deletion :** Assessment Template List and Issue Template List both are provided with an action button for deleting template. On clicking delete button from **Actions** column, a popover opens which asks for confirmation for deletion. On clicking **Ok** button, the selected template is deleted.
 3. **Search Bar :** Search bar allows user to search the required template out of the list by typing keyword.

         

 

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTgzMDQ5NjAzMCwxMTY0MzM5MjAsNjM5Nj
c3OTg5LC0yMDY2OTU1MDUxXX0=
-->