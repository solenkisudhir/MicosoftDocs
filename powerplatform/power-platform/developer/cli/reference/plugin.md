---
title: Microsoft Power Platform CLI plugin command group| Microsoft Docs
description: "Describes commands and parameters for the Microsoft Power Platform CLI plugin command group."
keywords: "pac cli"
ms.subservice: developer
author: snizar007
ms.author: snizar
ms.date: 11/10/2023
ms.reviewer: jdaly
ms.topic: reference
contributors: 
 - JimDaly
---
<!-- 
Do not edit this file. 
This file is generated by a program and any changes will be overwritten when this topic is re-generated.
Use the include files to add additional content to this topic.
-->
# pac plugin

Commands for working with Dataverse plug-in class library

[!INCLUDE [plugin-intro](includes/plugin-intro.md)]

## Commands

|Command|Description|
|---------|---------|
|[pac plugin init](#pac-plugin-init)|Initializes a directory with a new Dataverse plug-in class library.|
|[pac plugin push](#pac-plugin-push)|Import plug-in into Dataverse.|


## pac plugin init

Initializes a directory with a new Dataverse plug-in class library.

[!INCLUDE [plugin-init-intro](includes/plugin-init-intro.md)]


### Optional Parameters for plugin init

#### `--author` `-a`

One or more authors of the Dataverse Plug-in Package.

#### `--outputDirectory` `-o`

Output directory

#### `--signing-key-file-path` `-sk`

Relative path to the Dataverse plug-in assembly originator key file for signing.

#### `--skip-signing` `-ss`

Skip plug-in assembly signing that gives the plug-in assembly a strong name. The default value is 'false'.

This parameter requires no value. It's a switch.

[!INCLUDE [plugin-init-remarks](includes/plugin-init-remarks.md)]

## pac plugin push

Import plug-in into Dataverse.

[!INCLUDE [plugin-push-intro](includes/plugin-push-intro.md)]


### Required Parameters for plugin push

#### `--pluginId` `-id`

ID of plug-in assembly or plug-in package


### Optional Parameters for plugin push

#### `--configuration` `-c`

Build configuration. The default value is: 'Debug'.

#### `--pluginFile` `-pf`

File name of plug-in assembly or plug-in package

#### `--type` `-t`

Type of item if not specified explicitly through --pluginFile. The default value is: 'Nuget'.

Use one of these values:

- `Nuget`
- `Assembly`

[!INCLUDE [plugin-push-remarks](includes/plugin-push-remarks.md)]

[!INCLUDE [plugin-remarks](includes/plugin-remarks.md)]

### See also

[Microsoft Power Platform CLI Command Groups](index.md)<br />
[Microsoft Power Platform CLI overview](../introduction.md)