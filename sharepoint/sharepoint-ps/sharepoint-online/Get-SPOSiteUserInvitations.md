---
external help file: sharepointonline.xml
Module Name: Microsoft.Online.SharePoint.PowerShell
online version: https://learn.microsoft.com/powershell/module/sharepoint-online/get-spositeuserinvitations
applicable: SharePoint Online
title: Get-SPOSiteUserInvitations
schema: 2.0.0
author: techwriter40
ms.author: pamgreen
ms.reviewer:
---

# Get-SPOSiteUserInvitations

## SYNOPSIS

Searches against all stored sharing links and retrieves the email invites. 

## SYNTAX

```powershell
Get-SPOSiteUserInvitations [-Site] <SpoSitePipeBind> [-EmailAddress] <string> [<CommonParameters>]
```

## DESCRIPTION

Searches against all stored sharing links on a Site and retrieves the email invites. 

## EXAMPLES

### Example 1

```powershell
Get-SPOSiteUserInvitations -Site https://contoso.sharepoint.com/sites/ContosoWeb1/ -EmailAddress someone@example.com
```

This example retrieves email invites stored in the ContosoWeb1 site to the user with email address someone@example.com.

## PARAMETERS

### -Site

Specifies the URL of the site collection.

```yaml
Type: SpoSitePipeBind
Parameter Sets: (All)
Aliases:
Applicable: SharePoint Online
Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EmailAddress

Email Address of the user.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: SharePoint Online
Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters

This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](https://go.microsoft.com/fwlink/p/?LinkID=113216).

## NOTES
