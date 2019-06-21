---
title: "OnPreStageChange Event (Client API reference) in Dynamics 365 for Customer Engagement| MicrosoftDocs"
ms.date: 11/20/2017
ms.service: crm-online
ms.topic: reference
applies_to: Dynamics 365 for Customer Engagement (online)
ms.assetid: 
author: msftman
ms.author: deonhe
manager: kvivek
search.audienceType: 
  - developer
search.app: 
  - D365CE
---
# OnPreStageChange Event (Client API reference)

[!INCLUDE[](../../../../includes/cc_applies_to_update_9_0_0.md)]

This event occurs **Before** the stage of a business process flow control changes. This event occurs after the user clicks the **Next Stage** or **Move to previous stage** buttons in the user interface or when a developer uses the `formContext.data.process.moveNext` or `formContext.data.process.movePrevious` methods. You can’t cancel the stage change using code in a handler for this event.

An execution context object is passed to event handlers for this event. You can use the [getEventArgs](../executioncontext/getEventArgs.md) method to retrieve an object that has the following methods:
- **getDirection**: Returns a string that is either “next” or “previous” to show the direction of the stage change.
- **getStage**: Returns a stage object. Except when the navigation moves to a new entity, the stage returned represents the destination stage object,that is, the next active stage. When the navigation moves to a new entity, the stage is the stage being navigated from, that is, the previous active stage object. More information: [Stage methods](../formContext-data-process.md#stage-methods).

## Methods supported for this event
- **formContext.data.process**.[addOnStageChange](../formcontext-data-process/eventhandlers/addOnStageChange.md) method to add event handlers for this event.
- **formContext.data.process**.[removeOnStageChange](../formcontext-data-process/eventhandlers/removeOnStageChange.md) method to remove event handlers for this event. 


