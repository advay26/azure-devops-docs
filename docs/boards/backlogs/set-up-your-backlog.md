---
title: Manage your project's backlogs and boards in Azure Boards
titleSuffix: Azure Boards
description: Learn how to configure your project's backlogs and boards. Also, learn to display user stories, issues, tasks, or other work items that your team wants to track.  
ms.custom: boards-backlogs    
ms.service: azure-devops-boards
ms.assetid: 
ms.author: chcomley
author: chcomley
ms.topic: how-to
monikerRange: '<= azure-devops'
ms.date: 04/01/2022
---

# Set up your project's backlogs and boards in Azure Boards

[!INCLUDE [version-lt-eq-azure-devops](../../includes/version-lt-eq-azure-devops.md)]

In most cases, you can start using your product and portfolio backlogs once your project is created. A default team gets created along with associated backlogs and boards. You can start adding work items to your product backlog using the [Backlog](create-your-backlog.md) or [Board](../boards/kanban-quickstart.md). 

However, you might need to ensure you've configured your backlogs and boards correctly. Ensure the configuration if you've added a team and want to start using the team backlogs and boards. Changes may be made to a project or team configuration over time. These changes can influence the work items that appear on your backlog and boards. 

For an overview of the tools associated with your team, see [Manage and configure team tools](../../organizations/settings/manage-teams.md).

## Prerequisites

[!INCLUDE [temp](../includes/prerequisites.md)]

## Default backlog and board work items

The first thing you need to understand is that your product **Backlog** and **Board** display work items that meet the following criteria:

::: moniker range="<=azure-devops"

- Work item type belongs to the Requirements category. The types differ depending on the process selected for your project:  
	- [Basic](../get-started/plan-track-work.md) : Issue, Backlog name=<strong>Issues</strong>  
	- [Agile](../work-items/guidance/agile-process.md): User Story, Backlog name=<strong>Stories</strong>  
	- [Scrum](../work-items/guidance/scrum-process.md): Product Backlog Item, Backlog name=<strong>Backlog items</strong> 
	- [CMMI](../work-items/guidance/cmmi-process.md): Requirement, Backlog name=<strong>Requirements</strong>  
- Work item <strong>Area Path</strong> matches one of the selected team's Area Paths
- Work item <strong>Iteration Path</strong> is under the team's Default Iteration Path

::: moniker-end

[!INCLUDE [temp](../includes/basic-process-note.md)] 

You can determine the work item types that belong to your Requirements category. Determine the items by [opening your product Backlog](create-your-backlog.md) and checking the product backlog name. 

::: moniker range="<=azure-devops"

> [!div class="mx-imgBorder"]
> ![Product backlog level, Backlog items, Stories, or Requirements](../sprints/media/assign-items-sprint/select-product-backlog-agile.png)

::: moniker-end

Look up your team's Area Path(s) and Iteration Paths. For more information, see [Define area paths and assign to a team](../../organizations/settings/set-area-paths.md) and 
[Define sprint paths and configure team iterations](../../organizations/settings/set-iteration-paths-sprints.md#list-team-iterations). 

<a id="sprint"></a>

## Default sprint backlog and Taskboard work items

Your sprint backlog and Taskboard apply the filters associated with your team's default backlog and board work items along with the Iteration Path you select.  

You can only select Iteration Paths that have been [preselected by your team](../../organizations/settings/set-iteration-paths-sprints.md#list-team-iterations). 

Your sprint backlog displays only those work items assigned to the selected sprint. Child tasks assigned to other sprints aren't displayed.  

## Review checklist for work items, backlogs, and boards

If you don't see the work items you expect on your [product Backlog](create-your-backlog.md) or [board](../boards/kanban-quickstart.md), complete the following checks: 

1. Make sure you've selected the team backlog or board of interest. To learn how, see [Use breadcrumbs and selectors to go to and open artifacts](../../project/navigation/use-breadcrumbs-selectors.md). 

2. [Create a query](../queries/using-queries.md) of your backlog items, specifying the work item types that belong to your Requirements category and the Area Path associated with your team, for example:  

	> [!div class="mx-imgBorder"]
	> ![Requirement category query](media/setup-backlog/requirements-query.png)

3. Add the <strong>State</strong>, <strong>Area Path</strong>, and <strong>Iteration Path</strong> fields to the [column options](set-column-options.md).

4. Check the query results and that the values of the work items you expect to show up on your backlog meet these criteria:
	- <strong>Area Path</strong> belongs to your team's area path(s)
	- <strong>Iteration Path</strong> belongs under your team's default iteration path
	- <strong>State</strong> isn't Closed, Completed, Done, or Removed. 

> [!NOTE]
> You can also filter your product backlog to show or hide work items that are in an **In Progress** state category, corresponding to an Active, Resolved, Committed, Doing workflow state. 

## Add bugs to your backlogs and boards

::: moniker range="<=azure-devops"

For all processes except the Basic process, each team manages the way bugs are tracked. Track bugs in the Requirements category because they show up on the Backlog and board or the Tasks category. They can also show up on the Taskboard or the Bugs category where they don't appear on either backlogs or boards. 

::: moniker-end

[!INCLUDE [temp](../includes/basic-process-bug-note.md)]

If you want bugs to show up on your Backlog and Board, choose <strong>Bugs are managed with requirements</strong>.

> [!div class="mx-imgBorder"]
> ![Working with bugs options](media/setup-backlog/working-with-bugs.png)

For more information, see [Show bugs on backlogs and boards](../../organizations/settings/show-bugs-on-backlog.md). 

## Correct your board configuration

If you see the following error when you open your board, you need to correct the configuration. The main reason for this error is that the workflow states of work item types that have been added to the Requirements category aren't mapped to the column. 

> [!div class="mx-imgBorder"]
> ![Board, Configuration error message](media/setup-backlog/column-config-error.png)

Choose **Correct this now** to open the Settings dialog. To map the workflow states, refer to [Add columns to your board, Update column-to-State mappings](../boards/add-columns.md#state-mappings). 

## Customize your board checklist items

Checklists are a great way to create work items that are automatically linked with a parent-child link to another work item on a board. You can customize the work item types that you can add as a checklist by opening the Board Settings, choose **Annotations**, and enable the work item types you want to appear on the board. For more information, see [Customize cards](../boards/customize-cards.md).

::: moniker range="<=azure-devops"

For example, here we've chosen to track bugs along with tasks, and  enable Task, Bug, GitHub objects, and Tests to appear within checklists. 

> [!div class="mx-imgBorder"]
> ![On the settings page, the Annotations tab is selected and four Annotation types, all enabled, are listed. They are: Task, Bug, GitHub, and Tests.](../boards/media/customize-cards/annotate-settings-154.png)

::: moniker-end

::: moniker range="<=azure-devops"

For more information about checklists, see the following articles: 
- [Add tasks or child items as checklists](../boards/add-task-checklists.md)  
- [Add, run, and update inline tests](../boards/add-run-update-tests.md)
- [Link GitHub commits, pull requests, branches, and issues to work items](../github/link-to-from-github.md)

::: moniker-end

<a id="customize-checklist-2019"></a>

## Add other work item types to your board checklist

If you added work item types to the Task Category as described in [Add custom work item types to your Taskboard](#taskboard-types) later in this article, you can choose if these types appear within a checklist on your product board. You make this choice by opening **Board Settings**, choose **Annotations**, and enable the work item types you want to appear on the board. You can enable up to five annotations. For more information, see [Customize cards](../boards/customize-cards.md). 

For example, here  we've chosen to track bugs along with tasks, and we enable Issue and Ticket and Task and Bug. For more information about checklists, see [Add tasks or child items as checklists](../boards/add-task-checklists.md) and [Add, run, and update inline tests](../boards/add-run-update-tests.md). 

> [!div class="mx-imgBorder"]
> ![On the settings page, the Annotations tab is selected and five Annotation types (Task, Bug, Tests, Issue, Ticket) are listed. All but Tests are enabled.](media/setup-backlog/annotations-on-prem.png)

## Hide or show backlog levels 

Your team can also choose to hide or show one or more backlog levels. Feature teams often manage backlog items, while management teams manage features and epics. In this situation, you can enable or disable a backlog level. 

> [!div class="mx-imgBorder"]
> ![Backlog navigation levels](media/setup-backlog/backlog-levels.png)

For more information, see [Select backlog navigation levels for your team](../../organizations/settings/select-backlog-navigation-levels.md). 

<a id="add-custom-types"></a>

## Add custom work item types to your backlogs and portfolio backlog levels  

If you want to track different work item types on your product backlog, you can do that by adding custom work item types and adding them to a specific backlog level. 

You can also add custom work item types and add them to portfolio backlogs. You can add up to five portfolio backlogs. 

For example, here we've added Initiatives, fourth level, and fifth level work item types to support five levels of portfolio backlogs. We've also added a custom work item type named Ticket and added that to the product backlog. 

> [!div class="mx-imgBorder"]
> ![Add custom work item types to your backlogs.](media/setup-backlog/backlog-levels-customized.png)

For more information, see the following resources: 

::: moniker range="azure-devops"

- [Add and manage work item types (Inherited process)](../../organizations/settings/work/customize-process-work-item-type.md)
- [Customize your backlogs or boards (Inherited process)](../../organizations/settings/work/customize-process-backlogs-boards.md) 
- [Customize an inheritance process](../../organizations/settings/work/inheritance-process-model.md)  

::: moniker-end

::: moniker range="<azure-devops"

**Inheritance process model:**  
- [Add and manage work item types (Inherited process)](../../organizations/settings/work/customize-process-work-item-type.md)
- [Customize your backlogs or boards (Inherited process)](../../organizations/settings/work/customize-process-backlogs-boards.md) 
- [Customize an inheritance process](../../organizations/settings/work/inheritance-process-model.md)  

**On-premises XML process model:**  
- [Add a work item type to a backlog and board](../../reference/add-wits-to-backlogs-and-boards.md)  
- [Add portfolio backlogs](../../reference/add-portfolio-backlogs.md)
- [Customize the On-premises XML process model](../../reference/on-premises-xml-process-model.md) 

::: moniker-end

<a id="taskboard-types"></a> 

## Add custom work item types to your Taskboard

To add custom work item types to appear on your sprint Taskboard, follow the steps outlined next based on the process model your project uses. 

::: moniker range="<=azure-devops"
> [!NOTE]
> You can enable work item types that you add to your Iteration backlog to appear as a checklist on your product board. To learn how, see [Customize your board checklist items](#customize-checklist-2019) provided earlier in this article. 

::: moniker-end

::: moniker range="<=azure-devops"

### Track custom work items with the Inherited process model 

For example, if you want to track a custom work item type, Tickets, along with Tasks and Bugs, you do the following tasks: 

1. Define the Ticket custom work item type. See [Add and manage work item types](../../organizations/settings/work/customize-process-work-item-type.md).

2. Add the Ticket work item types to the Iteration backlog. For more information, see [Customize your backlogs or boards for a process](../../organizations/settings/work/customize-process-backlogs-boards.md).  

::: moniker-end

::: moniker range="< azure-devops"

### Add existing and custom work item types with the On-premises XML process model 

For on-premises deployments that use the On-premises XML process model to customize work tracking, you can add existing and custom work item types to the sprint Taskboards. For example, if you want to track Issues (or Impediments for the Scrum process) and a custom work item type, Tickets, along with Tasks and Bugs, you would do the following tasks: 

1. Define the Ticket custom work item type. See [Add or modify a work item type](../../reference/add-modify-wit.md). 
2. Add Issue and Ticket work item types to the Task Category by modifying the Categories XML file. For more information, see [Categories XML element reference](/previous-versions/azure/devops/reference/xml/categories-xml-element-reference).  

	For example, here we add Issue and Ticket to the Task Category.  

	> [!div class="tabbedCodeSnippets"]
	> ```XML
	>   <CATEGORY name="Task Category" refname="Microsoft.TaskCategory">
	>     <DEFAULTWORKITEMTYPE name="Task" />
	> 	<WORKITEMTYPE name="Issue" / 
	> 	<WORKITEMTYPE name="Ticket" / 
	>   </CATEGORY>
	> ```

3. Make sure that the Issue and Ticket workflow states are mapped to category states. As needed, modify the ProcessConfiguration XML file to add Issues and Tickets to the `TaskBacklog` section. 

	For example, here the New, Active, and Closed states are mapped for the Task Category.

	> [!div class="tabbedCodeSnippets"]
	> ```XML
	>   <TaskBacklog category="Microsoft.TaskCategory" pluralName="Tasks" singularName="Task" workItemCountLimit="1000">
	>     <States>
	>       <State value="New" type="Proposed" />
	>       <State value="Active" type="InProgress" />
	>       <State value="Closed" type="Complete" />
	>     </States>
	> . . .
	>   </TaskBacklog>
	> ```

4. To verify your changes, open a Sprint backlog and make sure you can add an Issue or Ticket in the same way you add a Task. See [Add tasks](../sprints/add-tasks.md). 

::: moniker-end

## Other factors that can affect work items in your backlogs and boards
The following settings can influence the type and number of work items that appear in your backlogs and boards. 

- In your board, newly added work items may not appear if they're stack ranked lower within the product backlog. By choosing **Show more items**, you can cause the board to refresh and display more work items. 

	> [!div class="mx-imgBorder"]  
	> ![Boards, Show more items](media/setup-backlog/show-more-items.png) 

- If you have nested work items that belong to the same category, only leaf nodes may appear on the board (for TFS 2018.1 and earlier versions). For this reason, we recommend that you don't nest work items of the same work item type or belonging to the same category. For more information, see [Fix reordering and nesting issues, How backlogs and boards display hierarchical (nested) items](resolve-backlog-reorder-issues.md).

- If you've turned off the **In Progress** view, then those work items where work has started won't appear in the backlog list.  

	::: moniker range=">= azure-devops-2020"
	> [!div class="mx-imgBorder"]  
	> ![Backlogs, View Options, Hide In Progress](media/setup-backlog/hide-in-progress-s155.png)  
	::: moniker-end

	

	

- Work items appear in the priority order in which they're added or moved to. This order or sequence is managed by the **Stack Rank** (Basic, Agile, and CMMI processes) or **Backlog Priority** (Scrum) field. For more information, see the Stack rank section in [Backlogs, portfolios, and Agile project management](backlogs-overview.md#stack-rank).

- Each backlog can display up to 999 work items. If your backlog exceeds this limit, then you may want to consider adding a team and moving some of the work items to the other team's backlog.  

- Sprint backlogs show only those work items that meet the team's area path and the **Iteration Path** defined for the sprint. 

- Inheritance process model: If an administrator [disables or deletes a work item type](../../organizations/settings/work/customize-process-work-item-type.md#enable-disable), it doesn't appear on backlogs and boards. 

- On-premises XML process model: If an administrator [deletes or destroys a work item type](../../reference/witadmin/witadmin-import-export-manage-wits.md), it doesn't appear on backlogs and boards.

## Related articles

- [Add a team, move from one default team to several teams](../../organizations/settings/add-teams.md)
- [Create your backlog](create-your-backlog.md)
- [Backlog priority or stack rank order](backlogs-overview.md#stack-rank)
- [Use categories to group work item types](/previous-versions/azure/devops/reference/xml/use-categories-to-group-work-item-types)
- [Workflow states & state categories](../work-items/workflow-and-state-categories.md) 
- [Automate work item state transitions](../work-items/automate-work-item-state-transitions.md)
