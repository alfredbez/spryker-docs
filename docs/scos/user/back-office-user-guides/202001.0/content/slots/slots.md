---
title: Slots
description: The article provides some general information about slots and actions you can perform on them in the Back Office.
last_updated: Mar 26, 2020
template: back-office-user-guide-template
originalLink: https://documentation.spryker.com/v4/docs/slots
originalArticleId: c0aa47d1-c269-4cf1-a6c9-d0f43181a43e
redirect_from:
  - /v4/docs/slots
  - /v4/docs/en/slots
related:
  - title: Templates & Slots Feature Overview
    link: docs/scos/user/features/page.version/cms-feature-overview/templates-and-slots-overview.html
---

Slots are used to embed content into pages to which [templates with slots](/docs/scos/user/features/{{page.version}}/cms-feature-overview/templates-and-slots-overview.html) are applied.

In the Slots page, you can:
* overview the list of templates of Storefront pages;
* overview the list of slots;
* activate or deactivate slots.
* overview the list of CMS blocks assigned to a slot;
* assign CMS blocks to a slot;
* change the order of CMS blocks assigned to a slot;
* delete a CMS Block assignment;
* view an assigned CMS Block;
* select the pages in which a CMS Block is displayed.

On entering the page. the following is selected by default:
* The first template from the **List of Templates** is selected by default. Its slots are displayed in the **List of Slots for [name] Template**. Click on a different template to display the slots assigned to it.  
* The first slot from the **List of Slots for Template [name]** is selected by default. Its assigned CMS blocks are displayed in the **List of assigned Blocks for [name] Slot**. Click on a different slot to display the blocks assigned to it.
* The first CMS Block from the **List of Blocks for Slot [name]** is selected by default. In the **Product Pages** field, you can see the pages in which this CMS block is displayed. Click on a different CMS block to display its pages.

{% info_block warningBox "Integration required" %}

You can work with slots after the [Templates & Slots feature has been integrated](/docs/scos/dev/feature-integration-guides/{{page.version}}/cms-feature-integration.html) into your project.

{% endinfo_block %}

***

**What's next?**
* To learn how to add content to Storefront pages using Templates & Slots, see [Adding Content to Storefront Pages Using Templates & Slots](/docs/scos/user/back-office-user-guides/{{page.version}}/content/adding-content-to-storefront-pages-using-templates-and-slots-best-practices.html).
* To learn how to activate or deactivate slots, assign CMS blocks to a slot, change the order of CMS blocks assigned to a slot, delete an assignment or select the pages in which a CMS block is displayed, see [Managing Slots](/docs/scos/user/back-office-user-guides/{{page.version}}/content/slots/managing-slots.html).
* To learn about the attributes you can see in the **Slots** section, see the [Slots: Reference Information](/docs/scos/user/back-office-user-guides/{{page.version}}/content/slots/references/slots-reference-information.html) section.
