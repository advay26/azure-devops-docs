---
title: What is Azure Boards
titleSuffix: Azure Boards
description: Learn about the Agile tools that Azure Boards provides to manage software development projects.
ms.custom: boards-get-started
ms.subservice: azure-devops-new-user
ms.author: chcomley
author: chcomley
ms.topic: overview
monikerRange: '<= azure-devops'
ms.date: 04/21/2025
#customer intent: As a developer, I want to explore the Agile tools that Azure Boards provides, so I can manage software development projects.
---

# What is Azure Boards?

[!INCLUDE [version-lt-eq-azure-devops](../../includes/version-lt-eq-azure-devops.md)]

Azure Boards is a web-based service that enables teams to plan, track, and discuss work across the entire development process, while it supports [agile methodologies](../work-items/guidance/agile-process.md). Azure Boards provides a customizable platform for managing work items, allowing teams to [collaborate](../../cross-service/cross-service-overview.md) effectively and streamline their workflow. [Sign up](sign-up-invite-teammates.md), [customize](../configure-customize.md), and experience the [benefits of using Azure Boards](#benefits-of-using-azure-boards).
 
## Azure Boards hubs

You can track and manage work and access various functions within each of the following hubs.

|Azure Boards hub |Functions |
|-----------------|----------|
|[**Work items**](../work-items/about-work-items.md) | Access lists of work items based on specific criteria, such as those assigned to you, ones you follow, and work items you viewed or updated. |
|[**Boards**](../boards/kanban-overview.md) | View work items as cards and update their status through drag-and-drop, similar to physical sticky notes on a whiteboard. Use this feature to implement Kanban practices and visualize work flow for a team. |
|[**Backlogs**](../backlogs/backlogs-overview.md) | View, plan, order, and organize work items, including using a product backlog to represent your project plan and a portfolio backlog to group work under features and epics. |
|[**Sprints**](../sprints/assign-work-sprint.md) | Access your team's filtered view of work items based on a specific sprint or iteration path. Assign work to a sprint by using drag-and-drop from the backlog. implement Scrum practices by interacting with a backlog list or card-based Taskboard. |
|[**Queries**](../queries/view-run-query.md) | Generate custom work item lists and perform various tasks, such as triage work, make bulk updates, and view relationships between work items. Queries also allow for creating status and trend charts that can be added to dashboards. |
|[**Delivery Plans**](../plans/review-team-plans.md) | Management teams can view deliverables and track dependencies across multiple teams in a calendar view. Delivery plans support tasks such as viewing up to 15 team backlogs, custom portfolio backlogs and epics, and work that spans several iterations. Users can add backlog items to a plan, view rollup progress of features and epics, and dependencies between work items. |
| [**Analytics views**](../../report/powerbi/what-are-analytics-views.md) | Create highly sophisticated Power BI reports, based on Azure Boards data (work items). Access default Analytics views or create a custom view. |

**Azure Boards hubs UI**

:::image type="content" source="media/about-boards/boards-hubs.png" alt-text="Screenshot of hubs in Azure Boards menu, including Work items, Boards, Backlogs, Sprints, Queries, Delivery Plans, and Analytics views.":::

## Benefits of using Azure Boards

The following table lists some of the benefits of using Azure Boards.

|Benefit |Details |
|--------|--------|
|Start simply, scale as you grow | Azure Boards offers predefined work item types for tracking features, user stories, bugs, and tasks, making it easy to start using your product backlog or board. It supports different [Agile methods](../plans/agile-culture.md), so you can implement the method that suits you best. You can add teams as your organization grows to give them the autonomy to track their work as they see fit. |
|Use visual, interactive tools | Visual tools help teams quickly see and share progress with [Boards](../boards/kanban-quickstart.md), [product backlogs](../backlogs/create-your-backlog.md), [built-in scrum boards and planning tools](../sprints/scrum-overview.md), and [delivery plans](../plans/review-team-plans.md). |
|Customize easily |Easily [configure and customize](../configure-customize.md) boards, Taskboards, and delivery plans through the user interface, as well as add [custom fields, work item types, and portfolio backlogs](../../organizations/settings/work/inheritance-process-model.md). |
|Use built-in social tools and communication | [Work item forms](../work-items/about-work-items.md#work-item-form-controls) provide built-in discussion that you can use to capture questions, notes, and communication as they occur. You can maintain a history of what a team decides on any particular work item. You can also quickly bring a team member or an entire team into the conversation [by using @mentions](../../organizations/notifications/at-mentions.md). |
|Capture information, generous cloud storage | Work items are designed to track all the information you need. You can edit in rich text, drag and drop inline images, and add larger attachments - up to 60 MB and as many as 100. Also, you can [link work items](../backlogs/add-link.md) within a hierarchy or by simple related links. Each work item form maintains a history of changes, so you can review what changed, who made the change, and when. |
|Find what you need quickly and get notified of changes | Azure Boards provides easy-to-use tools to help you quickly find specific work items as your project grows. You can [follow work items](../work-items/follow-work-items.md) to monitor updates and changes, use pivot views to show work items assigned to you, use the [query engine](../queries/query-field-value.md) to filter work items based on any field, and use ad-hoc search with quick inline filters. You can also personalize your alerts for work items that are changed or assigned to you. |
|Monitor status and progress with built-in dashboards and analytics | With Azure Boards, you gain access to many tools to generate reports to support tracking status and trends. By using [configurable dashboards](../../report/dashboards/dashboards.md), you can add one or more widgets. You configure widgets to display the information and data you want, such as the following bug [burndown widget](../../report/dashboards/configure-burndown-burnup-widgets.md). Along with dashboards, you have access to the [Analytics service](../../report/powerbi/what-is-analytics.md). This service is optimized for fast read-access and server-based aggregations. By using [Analytics views](../../report/powerbi/what-are-analytics-views.md) and Power BI, you can create highly sophisticated reports on the project data of interest. |
|Integrate with Office | Project managers who want to use familiar tools can import and export work item queries to and from Microsoft Office Excel or import and export work items using .csv files. For more information, see [Bulk import or update work items using CSV files](../queries/import-work-items-from-csv.md) or [Bulk add or modify work items with Excel](../backlogs/office/bulk-add-modify-work-items-excel.md). |
|Extend functionality | You can gain even greater functionality by adding Marketplace extensions, many of which are free. An extension is an installable unit that adds capabilities to Visual Studio, Azure DevOps Services, or Visual Studio Code. You can find extensions within these products or in the [Visual Studio Marketplace](https://marketplace.visualstudio.com/azuredevops), Azure DevOps tab. Also, by using the [REST API](/rest/api/azure/devops/index), you can create your own extensions or tools to integrate with Azure DevOps Services. |
|Get updates via a mobile browser | It's easy to stay on top of changes as they occur, using the [mobile browser](../../project/navigation/mobile-work.md), you can be notified and respond to changes made to work items. |
|Start for free | You can start for free and add up to five free users and unlimited [stakeholders](../../organizations/security/get-started-stakeholder.md). |

For more information, see the [What is Azure Boards?](/training/modules/choose-an-agile-approach/3-what-is-azure-boards) Training module.

## Connect Azure Boards to GitHub

You can connect Azure Boards with GitHub repositories to link GitHub commits, pull requests, branches, and issues to work items. Use GitHub for software development and Azure Boards to plan and track work. Quickly open linked GitHub commits, pull requests, or issues from the board. For more information, see [GitHub & Azure Boards](../github/index.md).   

For more information, see [About default processes and process templates](../work-items/guidance/choose-process.md).

## Configure dashboards and Power BI reports 

Dashboards provide teams with customized views for status updates, progress tracking, and trend analysis. Teams can share information and improve workflows with flexible and tailored dashboard options.

:::image type="content" source="media/about-boards/dashboard.png" alt-text="Screenshot of Azure Boards Dashboards with Content Team status, Project Velocity, and Sprint Burndown information." lightbox="media/about-boards/dashboard.png":::   

Use Power BI to create customized reports based on Analytics service queries for quantitative analysis of project data. For more information, see [About dashboards, charts, reports, & widgets](../../report/dashboards/overview.md) and [What is the Analytics service?](../../report/powerbi/what-is-analytics.md).

## Gain visibility through end-to-end traceability

With Azure Boards, you gain the advantage of full integration with the Azure DevOps platform. Azure DevOps is designed to provide end-to-end traceability, tracking work from requirements to deployment. Gain insight at each step of decision making and software deployment. Some of the traceability tasks supported include: 
 
- Create a branch from a requirement
- Create a pull request of updated branch
- Validate the pull request using a build pipeline
- Create and run inline tests on requirements
- Merge the pull request into the main, default branch
- Deploy changes into production with deployment status to Azure Boards
- Monitor and report on requirements traceability

For more information, see [End-to-end traceability](../../cross-service/end-to-end-traceability.md) and [Cross-service integration and collaboration overview](../../cross-service/cross-service-overview.md).

## Support independent, autonomous teams 

A team in Azure Boards is a group of project members who work in a specific product area represented by hierarchical paths called **Area Paths**. Define teams by their name, members, and area paths and are essential for configuring Boards, Backlogs, Sprints, and Delivery Plans in Azure Boards. For more information, see [About teams and Agile tools](../../organizations/settings/about-teams-and-settings.md). 

:::image type="content" source="../../organizations/settings/media/agile-tools/agile-tools-team-assets.png" border="false" alt-text="Conceptual diagram of team tools that shows Team options for planning, tracking, collaboration, monitoring, and learning.":::   

Azure Boards integrates with popular chat tools such as [Microsoft Teams](../integrations/boards-teams.md) and [Slack](../integrations/boards-slack.md) through ChatOps. It also offers extensions that add new capabilities to your projects and can be found in the [Azure DevOps Marketplace](https://marketplace.visualstudio.com/azuredevops). These extensions can help with planning and tracking work items, sprints, scrums, and other project management tasks, as well as collaboration among team members. 

## New Azure Boards

You might notice some changes in the user experience of Azure Boards. These updates are part of the new Azure Boards, designed to provide a faster interface, improve accessibility, and ensure consistency with other areas of the product.

### What to expect

The core functionality of Azure Boards remains the same. It still contains the features you know and love such as Boards, Backlogs, Sprints, Queries, and Delivery Plans. However, the user experience is refined to align with the rest of Azure DevOps. User interface changes include increased spacing between elements and strategically placed scroll bars to enhance accessibility.

It can take time to adjust to changes. To ease the transition, try out the [new features](https://devblogs.microsoft.com/devops/new-boards-hub-rollout-update-2) exclusive to the updated Azure Boards.

### Provide feedback

If you encounter technical issues beyond the cosmetic, or want to provide feature input, [share your feedback](../../user-guide/provide-feedback.md) with the product team.

## Related content

- [Configure and customize Azure Boards](../configure-customize.md)
- [Explore the DevOps journey at Microsoft](https://azure.microsoft.com/solutions/devops/devops-at-microsoft/)
- [Promote an Agile culture](../plans/agile-culture.md)  
- [Learn about teams and Agile tools](../../organizations/settings/about-teams-and-settings.md)
