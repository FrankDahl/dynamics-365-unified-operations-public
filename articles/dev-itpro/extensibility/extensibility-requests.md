---
# required metadata

title: Extensibility requests
description: This topic explains how to file a request for additional extension points in Dynamics 365 for Finance and Operations. 
author: FrankDahl
manager: AnnBe
ms.date: 04/10/2018
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-platform
ms.technology: 

# optional metadata

# ms.search.form: 
# ROBOTS: 
audience: Developer
# ms.devlang: 
ms.reviewer: robinr
ms.search.scope: Operations
# ms.tgt_pltfrm: 
ms.custom: 89563
ms.assetid: 
ms.search.region: Global
# ms.search.industry: 
ms.author: fdahl
ms.search.validFrom: 2017-07-01
ms.dyn365.ops.version: Platform update 9
---

# Extensibility requests

[!include [banner](../includes/banner.md)]

Microsoft Dynamics 365 for Finance and Operations exclusively uses extensions to customize the product. We're aware that this change impacts our entire partner ecosystem. We recommend that you read the resources listed on the [Extensibility home page](extensibility-home-page.md). These resources answer many questions and prepare you for building solutions using extensions.

You will discover that some customizations, which were possible with overlayering, cannot be done through extensions. To enable the same business requirements without overlayering, we have added many extension capabilities and expect to add more going forward. For some customizations that were done with overlayering, you will need to log requests, to make us aware of what you need.

## What we are doing
We've been working toward an extension-based customization model for some time. Over the past several releases we have been gradually sealing models. As of Dynamics 365 for Finance and Operations release 8.0, this completes the sealing. From this release forward, only extension-based customizations are allowed. 

In future releases, we will be adding even more extensibility capabilities to enable independent software vendors (ISVs) and value-added resellers (VARs) to deliver complete business solutions. We will prioritize these on a customer-by-customer basis with frequent releases.

## How do I log extensibility requests?
If you discover a customization that you cannot implement as an extension, you must log a request to Microsoft to ensure appropriate extension support is added to the product for your scenario.

Before logging the request, there are a few things to consider:  
- Could the requirement be met with existing extensibility features? Building solutions with extensions requires different design and implementation patterns.
- How important is the requirement to the customer and/or business analyst?  
- Will the implementation be upgrade friendly for the long term?

Educate yourself on extensibility by reading up on resources published under the extensibility home page, and related sources.

As a partner, after you have signed the NDA agreements, people from your organization will be able to access the feedback Yammer groups. We recommend that you join the Yammer group 'Operations extensibility' where a broad range of extensibility topics are discussed.

Extensibility requests are logged using LCS under a project of choice. Requests that are logged are collected under the project they are logged. It is recommended that related requests are logged under the same LCS project as this help maintain a holistic view on all requests for a particular solution or an implementation.

> [!NOTE]
> Microsoft further identify logged requests by the organization name associated with the LCS account.

Navigate from within a LCS project to where extensibility requests are logged by selecting the Support menu item, then using clicking the tab.

![Extensibility support requests](media/extensibility-support-requests.png)

Here a list of already logged extensibility support requests show up. Each request will have a state that reflects how this is progressing. New requests that are logged will briefly list in **Pending** state, but only briefly while the request is copied to Microsoft tracking databases, and by this time an ID will be assigned the request, and this will list as **Active**. The ID can be clicked to review details of the logged request, here there is also an action to remove an active request in the even this is no longer required. There is currently no state available that can indicate feedback from Microsoft on when requests have been planned, but it is under consideration to add this. Requests that has been processed by Microsoft will show up with state **Closed**, and clicking the ID open information including resolution dates and description. Requests that have been closed release with monthly application updates.

The extensibility support request form includes two actions 'Create extensibility support request' and 'Manage extensibility options'. The 'Manage extensibility options' is where information that are common for all requests is maintained.

![Maintain extensibility support options](media/extensibility-options.png)

This is where information on your organization role is specified, like is this project including requests for either an **ISV** or **VAR** solution, or if requests are specific for a **Customer** implementation project. With the role **ISV** or **VAR** a field for entering Solution name must be specified, please enter a Solution name that is easily recognizable like to correlate with AppSource solutions. The 'Required by date' field is available to indicate the latest date by which requests are needed to become available for your development. Note there is no guarantee provided by Microsoft to that requests will be provided timely, but the required date provide an indication that will be considered when planning for requests at Microsoft.

Extensibility support options can be edited also after requests have been created. This is useful in cases like when plans for when requests is needed have changed, then please supply the information and click the 'Update' action to notify Microsoft to the update.

> [!NOTE]
> There is currently no option with the tool to record what Customer implementation includes in terms of ISV or VAR solutions. It is under consideration that this will be added.

The action 'Create extensibility support request' is used for creating new extensibility requests.

![Create extensibility support request](media/create-extensibility-request.png)

When you log extensibility requests, please enter detailed information about what you need to become enabled for extensibility and include information on what it is you need to extend. This will help Microsoft to be efficient in addressing your requests. You are welcome to propose how Microsoft could enable the functionality that you need in the standard application in a way that effectively addresses your needs.

Consider first the request type which is how we from Microsoft have categorized requests based from experience. Selecting request type will adjust the form to include specific fields related to the type. This is to help guide the process through supplying the information needed to make the request actionable for Microsoft.

Microsoft is very rarely enabling requests by adding inline delegates, so please consider other types of requests whenever feasible. Common application request types includes 'extract method', 'extensible enum', 'construct with throw', and 'method change'. There is also the request types 'platform request', and 'metadata change' for proposing changes like general platform improvements. The request type 'method signature change' is typically a request for a breaking change, and this is unlikely that it can be accommodated under monthly updates, but that it will require a more major release version to drive such changes.  

Take care in accurately entering element and method names for requests.

The form includes fields that only take text as input but notice also the action 'Attach file from computer' which can be used for uploading documents and attach these with requests. Do use attachments for supplying code snippets that may detail the request. Microsoft encourage that you are as specific as possible with your requests, so detailed proposals are very welcome.

Log request for each instance this is needed, and do not bundle multiple requests into one request. If multiple requests are related, then consider adding a document or description that include the ID's on these requests such that work on these are considered in context.

The requests include a point of contact. This is supplied for cases where the logged extensibility request is not actionable for one reason of another. The requests may be intrusive and require discussion how different design options. Microsoft will use this contact information and email out to the supplied contact email to drive such interactions.

Notice the privacy statement before logging requests.

The 'Submit' action will create the request. Notice requests cannot be edited once submitted, so take time to check data before submitting. Requests that are accidentally submitted with incomplete or inaccurate date can be removed using the designated action after clicking the ID on the request.

Requests that are submitted to Microsoft will temporarily show as with **Pending** state until the request is created within Microsoft tracking databases. This will assign an ID to the request and it will read state **Active**, this further indicate that the request is now visible to Microsoft.

> [!NOTE]
> We will not release extensibility requests as hotfixes.  

Extensibility requests are only released for the most current Dynamics 365 for Finance and Operations. We are not planning to accommodate extensibility requests for earlier versions of Dynamics 365 for Finance and Operations, Dynamics AX 2012 or earlier releases.

## When will my extensibility requests be enabled?

Extensibility requests are logged to a backlog. Microsoft engineers prioritize all requests, and then work on them in priority order. Please note that Microsoft is not ensuring that all requests will be fulfilled. In particular, requests that are intrusive by nature will not be supported, as they will prevent seamless upgrade.

## How will extensibility requests be made available to deploy?
After Dynamics 365 for Finance and Operations release 8.0, we plan to release frequent application updates with new extensibility requests. This will follow the same release cadence as platform updates. 

## Still have questions?

Read the [Extensibility FAQ](app-sealing-faq.md) and the other resources listed on the [Extensibility home page](extensibility-home-page.md).
