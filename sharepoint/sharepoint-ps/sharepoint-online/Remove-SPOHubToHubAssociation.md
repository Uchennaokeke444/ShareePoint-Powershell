---
external help file: sharepointonline.xml
Module Name: Microsoft.Online.SharePoint.PowerShell
online version: https://learn.microsoft.com/powershell/module/sharepoint-online/remove-spohubtohubassociation
applicable: SharePoint Online
title: Remove-SPOHubToHubAssociation
schema: 2.0.0
author: techwriter40
ms.author: pamgreen
ms.reviewer:
---

# Remove-SPOHubToHubAssociation

## SYNOPSIS

Removes the selected hub site from its parent hub.

## SYNTAX

```powershell
Remove-SPOHubToHubAssociation [-HubSiteId] <SpoHubSitePipeBind> [<CommonParameters>]
```

## DESCRIPTION

Use this cmdlet to remove the selected hub site from its parent hub.

## EXAMPLES

### Example 1

```powershell
Remove-SPOHubToHubAssociation -HubSiteId 6638bd4c-d88d-447c-9eb2-c84f28ba8b15
```

This example removes the site with the given id from its parent Hub.

## PARAMETERS

### -HubsiteId

Id of the Hub site to be removed from its parent Hub.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases:
Applicable: SharePoint Online
Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters

This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](https://go.microsoft.com/fwlink/p/?LinkID=113216).

## NOTES
