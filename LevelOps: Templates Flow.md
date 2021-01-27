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
         - On clicking this button user is navigated to [http://localhost:3000/#/admin/templates/assessment-templates/create](http://localhost:3000/#/admin/templates/assessment-templates/create) and a **Assessment Template Settings** modal opens up. This modal allows user to set **Name** of assessment template, select **Knowledge Base** from the knowledge base list, select **Tags** from tags list and toggle **Risk Scoring Enabled**. On clicking **Ok** button a basic skeleton of users new assessment template is created.
         
         - Now user can add more sections by clicking **Add Section** button on the left provided **Sections Column**. On clicking the button a new section is created . User can provide **Title**, **Description** and add **Questions** to the newly created section. On selecting option type from the list, which opens on clicking **Add question to your section** button, present at the bottom of the right column, a **Edit Question Modal**  opens for editing question. Here user can give title to question and options, added or remove options etc. Once user has done editing, on clicking **Ok** button new question is added to the section. 
         - User can also **Delete** or **Edit** newly created question by clicking on the three vertical dots provided at the top right corner of each question. On clicking **Edit**, **Edit Question Modal** opens.
         - Once, user has added all the sections, user can save the assessment template by clicking **Save** button which navigates the user back to [http://localhost:3000/#/admin/templates/assessment-templates](http://localhost:3000/#/admin/templates/assessment-templates) or can edit assessment settings by clicking **Settings** button which opens **Assessment Template Settings** modal. 
 
 3. User is presented with a table which has following four columns:
    - **Name :**
	    - On clicking any cell user navigated to [http://localhost:3000/#/admin/templates/assessment-templates/edit?questionnaire={id}](http://localhost:3000/#/admin/templates/assessment-templates/edit).  Here **id** is the id of clicked assessment template. On the current open page,  user can add more sections by clicking **Add Section** button on the left provided **Section Column**. On clicking the button a new section is created to which user can provide **Title**, **Description** and **Add questions** to your section . On selecting answer type from the list opened on clicking add question button provided at bottom of right provided **Section Edit Column**, a **Edit Question Modal**  opens for editing question. On clicking **Ok** button new question is added to the section. User can also **Delete** or **Edit** newly created question by clicking on the three vertical dots provided at the top right corner of each question.
         - Once, user has added all the sections, user can save the assessment template by clicking **Save** button which navigates the user back to [http://localhost:3000/#/admin/templates/assessment-templates](http://localhost:3000/#/admin/templates/assessment-templates) or can edit assessment settings by clicking **Settings** button  which opens **Assessment Template Settings** modal . This modal allows user to set **Name** of assessment template, select **Knowledge Base** from the knowledge base list, select **Tags** from tags list and toggle **Risk Scoring Enabled**. On clicking **Ok** button new settings are added. User can also export the selected assessment template by clicking on **Export** button.
     - **Updated on :** This column gives date of last updation.
     - **Tags :** This column gives info about tags added to the assessment.
     - **Actions :** This column is provided with actions namely **Clone**, **Export** and **Delete** the assessment template.
 4. User can filter the assessment list on the basis of tags, by clicking on filter button which offers, user a list of tags to select from. On selecting tags, filters are applied to the list.
## <a id="issue-templates"> Issue Template Flow :</a>
 1. On clicking  **Issue Templates** option, user is navigated to [http://localhost:3000/#/admin/templates/issue-templates](http://localhost:3000/#/admin/templates/issue-templates).
 2. Here user has one button at top right corner :
	 - **Add Issue Template :**
	   -  On clicking this button user is navigated to [http://localhost:3000/#/admin/templates/issue-templates/edit](http://localhost:3000/#/admin/templates/issue-templates/edit) which is **Configure Template** page. This page allows user to add custom fields and assessments to the ticket template.
	   - Here user can set/change settings of the issue templates by clicking **Settings** button at the top right corner. A **Settings Modal** opens with allows user to toggle **Enable**, make current issue template **Default** once enabled, set **Name** and **Description** of Template. On clicking **Ok** button, settings are applied.
	   - On the left column user is provided with three panels:
		   - **Assessments :** This allows user to select assessment from list of available assessments.
		   - **Workflow Metadata :** This allows user to select type of metadata fields from the following:
			   - Single Dropdown
				- Multi Dropdown
			    - Dynamic Single Dropdown    
				- Dynamic Multi Dropdown
			   - Radio
		     - Text
			 - Text Area
			  - Date 
			- **Notifications :** This allows user to select multi ways of getting notified on **Email** or **Slack** or both.
		- Right Column is divided into two rows :
			- **Default Metadata Fields :** This row allows user to include/exclude default metadata fields by checking provided checkboxes adjacent to every field.
			- **Add Additional Metadata fields :** On clicking type of metadata field from **Workflow Metadata**, that particular field is added here. User can edit field settings or delete the field, by hovering over three vertical dots at the top right corner of each field. This provides user with two options:
				- **Settings :** On clicking this option, **Field Setting Modal** opens. User can mark the field **Hidden** or **Required**,  change **Label** or **Type** etc. On clicking **Ok** button settings are applied.
				- **Delete :** Clicking this option deletes the field.
		- Once user has set Template name in **Settings**, **Save** button is enabled and now user can save issue template. On clicking save button user is navigated back to [http://localhost:3000/#/admin/templates/issue-templates](http://localhost:3000/#/admin/templates/issue-templates).
 3. User is presented with a table which has following five columns:
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
eyJoaXN0b3J5IjpbLTc2NTcyNDIyNywtMjA2Njk1NTA1MV19
-->