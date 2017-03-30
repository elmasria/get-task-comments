# Get Comments from Workflow Tasks List

Helps to get the task comments from **Workflow Tasks** list


## Installation

1. clone repository or download as zip file
	* git clone ```https://github.com/elmasria/get-task-comments.git```

2. navigate to repository cd get-task-comments

3. Open required Sharepoint site

	1. Select settings
	2. Nintex Workflow 2013
	3. Manage User Defined Actions

4. Create UDA
	* Using UDA
		* Click Import
		* Select Get_Task_Comments.uda
	* Using Workflow
		* Click Create
		* Import
		* Select ```Get_Task_Comments.nwf```
		* Publish

## How To?

Users may use that **UDA** in the workflows, by drag and drop that Action.

### Configuration

1. paramDepartmentName: return the comments labeled by the time and the value you specified
2. paramPreviousComments: you may use that to concatenate the comments
3. paramTaskID: ID of the task that you need to get the value of the comment form it
4. paramSiteURL: the current site you work with. (by default you can use **Workflow Context** ==> **Web URL**)
	* this is helpful when you promote the UDA to be used in the **Farm Scope**
5. paramTaskListName: name of the list that contains the workflow tasks(by default it is  **Workflow Tasks**)
6. paramAllComments: variable that will hold the retrieved comments (**Multiple lines of text**)