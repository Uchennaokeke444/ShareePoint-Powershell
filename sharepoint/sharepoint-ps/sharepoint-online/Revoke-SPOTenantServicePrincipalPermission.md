---
external help file: sharepointonline.xml
Module Name: Microsoft.Online.SharePoint.PowerShell
online version: https://learn.microsoft.com/powershell/module/sharepoint-online/revoke-spotenantserviceprincipalpermission
applicable: SharePoint Online
title: Revoke-SPOTenantServicePrincipalPermission
schema: 2.0.0
author: trent-green
ms.author: trgreen
ms.reviewer:
---
# Revoke-SPOTenantServicePrincipalPermission

## SYNOPSIS

Revokes a permission that was previously granted to the "SharePoint Online Client" service principal

## SYNTAX

### Default

```powershell
Revoke-SPOTenantServicePrincipalPermission [-ObjectId] <String> [-Confirm] [<CommonParameters>]
```

## DESCRIPTION

Revokes a permission that was previously granted to the "SharePoint Online Client" service principal.

## EXAMPLES

### ------------------EXAMPLE 1------------------

```powershell
$grants = Get-SPOTenantServicePrincipalPermissionGrants
$grantToRemove = $grants | ? { $_.Resource -eq 'Office 365 SharePoint Online' -and $_.Scope -eq 'MyFiles.Read' } | Select-Object -First 1

if ($grantToRemove -ne $null)
{
    Revoke-SPOTenantServicePrincipalPermission -ObjectId $grantToRemove.ObjectId
}
```

Revokes the permission associated with the 'Office 365 SharePoint Online' resource and with scope claim 'MyFiles.Read'.
If there is no permission with those properties, then no revoke action will be taken.

## PARAMETERS

### -ObjectId

The Object ID of the permission grant to revoke

```yaml
Type: string

Required: True
Position: Named
Accept pipeline input: False
```

### -Confirm

Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf
Applicable: SharePoint Online
Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters

This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](https://go.microsoft.com/fwlink/p/?LinkID=113216).
