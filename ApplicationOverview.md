# Braintree Fixed Assets Maintenance

Braintree Fixed Assets Maintenance extends Microsoft Dynamics 365 Business Central with tools for maintaining fixed assets throughout their operating life. It brings asset maintenance planning, defect reporting, work execution, asset movements, usage tracking, and rental processing together with Business Central fixed-asset, purchasing, inventory, resource, and sales records.

## Maintenance setup and asset information

The application adds maintenance details to fixed assets, including a maintenance group, maintenance location, primary operator, usage unit of measure, and time- or usage-based maintenance intervals. A fixed asset can also be associated with an item and rental contract. Maintenance groups categorize assets and can identify a maintenance manager.

Administrators can configure number series for maintenance plans, maintenance orders, checklists, and asset transfers. Setup also provides access to maintenance groups, plan types, actions, measurements, and maintenance-order approval workflow configuration.

## Maintenance plans and scheduled work

Maintenance plans define reusable work for a maintenance group or an individual fixed asset. A plan can include:

- Ordered task lines with actions, components, measurement parameters, instructions, target values, tolerances, responsibility, and assigned resources.
- Planned expense/resource lines for items, G/L accounts, resources, vendors, and related costs.
- A maintenance plan type and time- or usage-based frequency.

Plans can be copied from existing plans and moved between Open, Released, and Blocked states. A processing report generates maintenance orders for selected plans and assets over a requested date range, using the plan's time frequency.

## Maintenance orders

Maintenance orders can be created directly, generated from plans, or initiated from a reviewed defect. An order contains work details, assigned resources, planned expenses, completion information, usage, and comments. Users can copy the plan's tasks and resources onto an order, create vendor purchase orders for vendor-linked resource lines, and use Business Central approval actions where an approval workflow is configured.

Posting a released order:

1. Posts item consumption, G/L maintenance costs, and resource usage to their respective Business Central journals.
2. Adds a maintenance registration against the fixed asset.
3. Adds or updates the asset's usage measurement for the completion date.
4. Marks the maintenance order Closed and records its completion date and user.

## Defect reporting and review

Users can register a defect against a fixed asset, identify a component and fault code, enter a detailed description, record usage, and attach a picture. The selected asset supplies its maintenance group and may suggest a reviewer; the fault code can supply a description and recommended action.

Defects move through New, Submitted, Under Review, Pending Correction, and Closed states. Authorized reviewers can add comments and choose a recommendation, including scheduling a repair, deferring action, or closing without action. Scheduling a repair creates a maintenance order from the selected maintenance plan. Review and close permissions are controlled through user setup.

## Asset transfers and usage

Fixed-asset transfer orders support movement between asset locations through an in-transit location. The Release, Ship, and Receive steps update transfer status and asset location, and record shipment and receipt movements in the application's asset movement ledger.

Asset usage can be viewed by asset and date. Maintenance-order posting records usage against the asset, allowing operational usage history to be reviewed alongside maintenance activity.

## Rental contracts

The rental functionality extends sales documents with rental-contract processing. It supports assigning serial-tracked inventory to rental assets, linking rental lines and fixed assets to a contract, and creating fixed-asset records from items using rental-related asset setup. Contract processing supports shipment and rental-period invoicing for eligible lines.

## Fixed-asset analysis

The FA Posting Group Analysis page summarizes fixed-asset ledger amounts by posting group and depreciation book. Users can filter by depreciation book, posting group, and posting date, and refresh the results to review acquisition cost, depreciation, disposal amounts, and book value.

## Role centre

The Braintree Asset Management role centre provides shortcuts to fixed assets, plans, orders, defects, usage, and planned-order generation. Activity cues summarize defect and maintenance-order states and fixed-asset transfer stages. It also provides access to maintenance registration history and related Business Central purchasing pages.

## Business Central records used

The application works with standard Business Central fixed assets and depreciation books, locations, items and inventory journals, G/L accounts and journals, resources and resource journals, vendors and purchase orders, sales documents, and user setup. Its permissions and workflow configuration determine which users can access maintenance data and perform restricted defect-review actions.
