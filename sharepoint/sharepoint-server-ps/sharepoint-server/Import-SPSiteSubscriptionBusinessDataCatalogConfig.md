---
external help file: Microsoft.SharePoint.PowerShell.dll-help.xml
module name: SharePointServer
online version: https://learn.microsoft.com/powershell/module/sharepoint-server/import-spsitesubscriptionbusinessdatacatalogconfig
applicable: SharePoint Server Subscription Edition
title: Import-SPSiteSubscriptionBusinessDataCatalogConfig
schema: 2.0.0
---

# Import-SPSiteSubscriptionBusinessDataCatalogConfig

## SYNOPSIS

Imports data associated with an exported file that contains all data associated with the Business Data Connectivity Metadata Store for a given partition.



## SYNTAX

```
Import-SPSiteSubscriptionBusinessDataCatalogConfig -Path <String> -ServiceContext <SPServiceContextPipeBind>
 [-AssignmentCollection <SPAssignmentCollection>] [-Confirm] [-LocalizedNamesIncluded] [-ModelsIncluded]
 [-PermissionsIncluded] [-PropertiesIncluded] [-ProxiesIncluded] [-WhatIf] [<CommonParameters>]
```

## DESCRIPTION
Use the Import-SPSiteSubscriptionBusinessDataCatalogConfig cmdlet to import a data file that contains Business Data Connecitivity models and all data associated with the Business Data Connectivity Metadata Store for a given partition.

For permissions and the most current information about Windows PowerShell for SharePoint Products, see the online documentation at [SharePoint Server Cmdlets](https://learn.microsoft.com/powershell/sharepoint/sharepoint-server/sharepoint-server-cmdlets).

## EXAMPLES

### ---------------------EXAMPLE--------------------------- 
```powershell
Import-SPSiteSubscriptionBusinessDataCatalogConfig -Path "C:\folder\importFile.xml" -ServiceContext http://contoso
```

This example imports the data file named importFile.xml.

## PARAMETERS

### -Path
Specifies the path and name to use to create the export file.The type must be a valid path in either of the following forms:

C:\folder_name

\\\\server_name\folder_name

..\folder_name\file.xml

```yaml
Type: String
Parameter Sets: (All)
Aliases: 
Applicable: SharePoint Server Subscription Edition

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServiceContext
Specifies the service context of the data to be exported.

The type must be a valid GUID, in the form 12345678-90ab-cdef-1234-567890bcdefgh; a valid name of a service context (for example, http://ServiceContext1); or an instance of a valid SPServiceContext object.

```yaml
Type: SPServiceContextPipeBind
Parameter Sets: (All)
Aliases: 
Applicable: SharePoint Server Subscription Edition

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AssignmentCollection
Manages objects for the purpose of proper disposal.
Use of objects, such as SPWeb or SPSite, can use large amounts of memory and use of these objects in Windows PowerShell scripts requires proper memory management.
Using the SPAssignment object, you can assign objects to a variable and dispose of the objects after they are needed to free up memory.
When SPWeb, SPSite, or SPSiteAdministration objects are used, the objects are automatically disposed of if an assignment collection or the Global parameter is not used.

When the Global parameter is used, all objects are contained in the global store.
If objects are not immediately used, or disposed of by using the Stop-SPAssignment command, an out-of-memory scenario can occur.

```yaml
Type: SPAssignmentCollection
Parameter Sets: (All)
Aliases: 
Applicable: SharePoint Server Subscription Edition

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before executing the command.
For more information, type the following command: `get-help about_commonparameters`

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf
Applicable: SharePoint Server Subscription Edition

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LocalizedNamesIncluded
Specifies that names for business data fields in multiple languages be imported.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Applicable: SharePoint Server Subscription Edition

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ModelsIncluded
Specifies that Business Data Connectivity models be included in the imported file.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Applicable: SharePoint Server Subscription Edition

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PermissionsIncluded
Specifies that permissions from the  Business Data Connectivity model be exported.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Applicable: SharePoint Server Subscription Edition

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PropertiesIncluded
Specifies that properties from the Business Data Connectivity model be imported.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Applicable: SharePoint Server Subscription Edition

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProxiesIncluded
Specifies that proxies for Business Data Connectivity Service Applications be exported.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Applicable: SharePoint Server Subscription Edition

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Displays a message that describes the effect of the command instead of executing the command.
For more information, type the following command: `get-help about_commonparameters`

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi
Applicable: SharePoint Server Subscription Edition

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (https://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
