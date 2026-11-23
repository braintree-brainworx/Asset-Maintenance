---
layout: NewLayout
title: Business Central for Asset Managers
description: Enhanced functionality for fixed asset management in Microsoft Dynamics 365 Business Central
---

# Setup and Configuration
Before using fixed asset maintenanceFor most of these, some default setups will be automatically be done when you install the app, allowing you to get started with a minimum of time and effort. Other setups will require your specific intervention. Either way, it's a good idea to review the setups, and adjust as required to match your own preferences.

- [Maintenance Setup](#setup-and-configuration)
- [Definitions](#definitions)
- [Measurements](#maintain-measurements)
- [Maintenance Actions](#maintenance-actions)
- [Maintenance Plan Types](#maintenance-plan-types)
- [Maintenance Group](#maintenance-groups)

## Fixed Assets Maintenance Setup
Search for 'FA Maintenance Setup', or select 'Maintenance Setup' from the Fixed Assets Setup page.

On installation, number series will be created for
- Maintenance plans
- Maintenance orders
- Checklists
- Transfers
- Rental Contracts
- Rental Asset Numbers

![alt text](Screenshots/FAMaintSetup.png)

You can amend these if required.

## Definitions
Definition of terms and entities used in the app:

| **Term** | **Definition** |
|---|---|
|Measurements|Defines key measurements taken as part of maintenance and inspections. |
|Maintenance Actions|Defines actions that are used in maintenance activities, for example Check, Top up, Adjust|
|Maintenance Group|Defines a group for which common maintenance activities apply, for example Passenger Vehicles, Motorcycles, Fridges|
|Maintenance Plan Types|Defines categories of maintenance plans, for example Minor Service, Safety Certification|
|Maintenance Plans|Defines a set of standard activities and resource requirements for the maintenance of a particular group of assets|
|Maintenance Order|Defines specific maintenance actions|
|Checklist||
|Defect Register ||

## Maintain Measurements
From FA Maintenance Setup, select 'Measurements'.
From the Measurements list, add or edit the entries. 

*Example:*
![alt text](/Screenshots/Measurements.png)

## Maintenance Actions
From FA Maintenance Setup, select 'Maintenance Actions'.
From the Maintenance Actions list, add or edit the entries.

    Note: it is not necessary to predefine all actions. They can be dynamically added during creation of maintenance plans.

## Maintenance Plan Types
Maintenance plan types define broad categories of maintenance, for example inspection, minor service, major service, safety compliance. 

From FA Maintenance Setup, select 'Maintenance Plan Types'.
From the Maintenance Plan Types list, add or edit the entries:

![alt text](/Screenshots/MaintenancePlanTypes.png)

Enter a code and description, and select a maintenance category from the available list.
Optionally, add the person responsible for managing the maintenance of assets belo

## Maintenance Groups
Maintenance groups are used to group a set of fixed assets together, based on common properties. The group can be used to associate typical maintenance activities with specific assets.

*Example*: 
Motor vehicles can be split by size and fuel type - Passenger Petrol, Passenger Diesel.

From FA Maintenance Setup, select 'Maintenance Groups'.
From the Maintenance Groups list, add or edit the entries:

![alt text](/Screenshots/MaintenanceGroups.png)

### Associating Maintenance groups with Maintenance Plan types
You can associate plan types with maintenance groups. Select 'Maintenance Plan Types' from the Maintenance Groups page.

![alt text](/Screenshots/MaintenancePlanTypes.png)

### Associating Maintenance Groups with Fixed Assets Subclasses
After you have created maintenance groups, you can link then to fixed asset subclasses. When a new asset is created and linked to a subclass, the maintenance group will be automatically assigned to the asset.

From the FA Maintenance Setup page, select 'Asset Subclasses':

![alt text](Screenshots/image.png)

In the column 'Maintenance Groups', select a maintenance group:

![alt text](Screenshots/image-1.png)