---
title: FAQs for AI suggestions for cases, knowledge articles | MicrosoftDocs
description: FAQs for AI suggestions for cases and knowledge articles in Dynamics 365 Customer Service.
author: neeranelli
ms.author: nenellim
manager: shujoshi
ms.date: 08/03/2020
ms.topic: article
ms.service: 
  - dynamics-365-customerservice
ms.custom: 
  - dyn365-customerservice
search.audienceType: 
  - admin
search.app: 
  - D365CE
  - D365CS
---

# Preview: FAQs on AI suggestions for cases and knowledge articles

[!include[cc-beta-prerelease-disclaimer](../includes/cc-beta-prerelease-disclaimer.md)]

A few answers to common questions on the AI-suggested similar cases and knowledge articles are listed here.

## I’ve enabled suggestions, but smart assist keeps showing me "No suggestions found" message

It may be caused by one of the following reasons:

- If it’s the first time you've enabled suggestions, it may take up to 24 hours to complete the pre-processing from your existing published knowledge articles and resolved cases before suggestions will be displayed.
- For the public preview release, the first time pre-process operation handles up to 3000 published knowledge articles and 50000 resolved cases from the most recent ones. Older articles and resolved cases are not picked up from the first time pre-processing, so they won’t be surfaced as suggestions.
- Suggestions are displayed for only active cases. Suggestions are updated when an active case is created or updated.
- The case title or description is not clear enough to describe the problem, therefore, the model can't find articles or similar cases that match what's described.
- Only English content is supported. For knowledge articles, the locale must be English.

## I've added more details about the problem in an active case, but the suggestions are not refreshed at all

In the public preview release, it may take one minute or more to get suggestions updated. You also are required to reopen the case form to see new suggestions.

## I’ve disabled the suggestions feature, but the suggestions still show up in Customer Service workspace

You need to refresh the browser for the settings to take effect.

## I can’t see smart assist with suggestions expanded at all when I open a case

Make sure that the case is opened in a session tab. To open it in a session tab, select the case using Shift+mouse click.

### See also

[Enable AI-suggestions for similar cases and knowledge articles ](csw-enable-ai-suggested-cases-knowledge-articles.md)  
[View AI-suggested similar cases and knowledge articles](csw-view-ai-suggested-cases-knowledge-articles.md)  