---
title: Table Filter Date Range
description: This document provides details about the Table Filter Date Range component in the Components Library.
template: concept-topic-template
---

This document explains the Table Filter Date Range component in the Components Library.

## Overview

Table Filter Date Range is a feature of the Table Component that allows filtering data via `Date Range Picker` component.

Check out an example usage of the Table Filter Date Range in the `@spryker/table` config.

Component configuration:

- `enabled` - enables the filter via config.  
- `items` - an array with config for each filter date-range.  

```html
<spy-table 
    [config]="{
        dataSource: { ... },
        columns: [ ... ],
        filters: {
            enabled: true,
            items: [
                {
                    id: 'range',
                    title: 'Range',
                    type: 'date-range',
                    typeOptions: {
                        placeholderFrom: 'from',
                        placeholderTo: 'to',
                    },
                },
            ],
        },                                                                                           
    }"
>
</spy-table>
```

## Component registration

Register the component:

```ts
// Dynamic
@NgModule({
    imports: [
        TableModule.forRoot(),
        TableModule.withFeatures({
            filters: () =>
                import('@spryker/table.feature.filters').then(
                    (m) => m.TableFiltersFeatureModule,
                ),
        }),
        TableFiltersFeatureModule.withFilterComponents({
            'date-range': TableFilterDateRangeComponent,
        }),
        TableFilterDateRangeModule,
    ],
})
export class RootModule {}
```

```html
// Via HTML
@NgModule({
    imports: [
        TableModule.forRoot(),
        TableFiltersFeatureModule,
        TableFilterDateRangeModule,
    ],
})
export class RootModule {}

<spy-table [config]="config">
    <spy-table-filters-feature spy-table-feature></spy-table-filters-feature>
</spy-table>
```

## Interfaces

Below you can find interfaces for the Table Filter Date Range:

```ts
declare module '@spryker/table.feature.filters' {
    interface TableFiltersRegistry {
        dateRange: TableFilterDateRange;
    }
}

export interface TableFilterDateRange
    extends TableFilterBase<DateRangeValueInput> {
    type: 'date-range';
    typeOptions: TableFilterDateRangeOptions;
}

export interface TableFilterDateRangeOptions {
    placeholderFrom?: string;
    placeholderTo?: string;
    format?: string;
    time?: string | boolean;
}
```
