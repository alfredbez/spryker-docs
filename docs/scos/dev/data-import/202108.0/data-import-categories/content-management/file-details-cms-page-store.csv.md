---
title: File details- cms_page_store.csv
last_updated: Jun 16, 2021
template: data-import-template
originalLink: https://documentation.spryker.com/2021080/docs/file-details-cms-page-storecsv
originalArticleId: e8f80649-24da-450a-a696-c3b9f02a52eb
redirect_from:
  - /2021080/docs/file-details-cms-page-storecsv
  - /2021080/docs/en/file-details-cms-page-storecsv
  - /docs/file-details-cms-page-storecsv
  - /docs/en/file-details-cms-page-storecsv
---

This article contains content of the **cms_page_store.csv** file to configure CMS Page Store information on your Spryker Demo Shop.

## Headers & Mandatory Fields 
These are the header fields to be included in the .csv file:

| Field Name | Mandatory | Type | Other Requirements/Comments | Description |
| --- | --- | --- | --- | --- |
| **page_key** | Yes (*unique*) | String |N/A* | Unique identifier of the page. |
| **store_name** | Yes | String |N/A | Store name identifier. |
*N/A: Not applicable.

## Dependencies

This file has the following dependencies:
*     [cms_page.csv](/docs/scos/dev/data-import/{{page.version}}/data-import-categories/content-management/file-details-cms-page.csv.html)
*     *stores.php* configuration file of the demo shop PHP project

## Template File & Content Example
A template and an example of the *cms_page_store.csv*  file can be downloaded here:

| File | Description |
| --- | --- |
| [cms_page_store.csv template](https://spryker.s3.eu-central-1.amazonaws.com/docs/Developer+Guide/Back-End/Data+Manipulation/Data+Ingestion/Data+Import/Data+Import+Categories/Content+Management/Template+cms_page_store.csv) | CMS Page Store .csv template file (empty content, contains headers only). |
| [cms_page_store.csv](https://spryker.s3.eu-central-1.amazonaws.com/docs/Developer+Guide/Back-End/Data+Manipulation/Data+Ingestion/Data+Import/Data+Import+Categories/Content+Management/cms_page_store.csv) | CMS Page Store .csv file containing a Demo Shop data sample. |

