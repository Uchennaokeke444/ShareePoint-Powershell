---
external help file: sharepointonline.xml
Module Name: Microsoft.Online.SharePoint.PowerShell
online version: https://learn.microsoft.com/powershell/module/sharepoint-online/set-spositedesign
applicable: SharePoint Online
title: Set-SPOSiteDesign
schema: 2.0.0
author: trent-green
ms.author: trgreen
ms.reviewer:
---

# Set-SPOSiteDesign

## SYNOPSIS

Updates a previously uploaded site design.

## SYNTAX

```powershell
Set-SPOSiteDesign
  [-Identity <SPOSiteDesignPipeBind>]
  [-Title <string>]
  [-WebTemplate <string>]
  [-SiteScripts <SPOSiteScriptPipeBind[]>]
  [-Description <string>]
  [-ThumbnailUrl <string>]
  [-PreviewImageUrl <string>]
  [-PreviewImageAltText <string>]
  [-IsDefault]
  [<CommonParameters>]
```

## EXAMPLES

### Example 1

This example updates a previously created site design.

```powershell
Set-SPOSiteDesign `
  -Identity 44252d09-62c4-4913-9eb0-a2a8b8d7f863 `
  -Title "Contoso customer tracking - version 2" `
  -WebTemplate "68" `
  -Description "Updated site design for list schema that tracks key customer data in a list" `
  -ThumbnailUrl "https://contoso.sharepoint.com/SiteAssets/site-thumbnail.png" `
  -PreviewImageUrl "https://contoso.sharepoint.com/SiteAssets/site-preview.png" `
  -PreviewImageAltText "site preview - version 2"
```

## DESCRIPTION

Updates a previously uploaded site design.

## PARAMETERS

### -Identity

The site design Id.

```yaml
Type: SPOSiteDesignPipeBind
Parameter Sets: (All)
Aliases:
Applicable: SharePoint Online
Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Title

The display name of the site design.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: SharePoint Online
Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WebTemplate

Identifies which base template to add the design to. Use the value **64** for the Team site template, and the value **68** for the Communication site template.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: SharePoint Online
Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SiteScripts

An array of one or more site scripts. Each is identified by an ID. The scripts run in the order listed.

```yaml
Type: SPOSiteScriptPipeBind[]
Parameter Sets: (All)
Aliases:
Applicable: SharePoint Online
Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description

The display description of the site design.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: SharePoint Online
Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ThumbnailUrl

The URL of a thumbnail image. If none is specified, SharePoint uses a generic image. Recommended size is 400 x 300 pixels.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: SharePoint Online
Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PreviewImageUrl

The URL of a preview image. If none is specified, SharePoint uses a generic image.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: SharePoint Online
Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PreviewImageAltText

The alt text description of the image for accessibility.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: SharePoint Online
Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IsDefault

A switch that if provided, applies the site design to the default site template. For more information, see [Customize a default site design](https://learn.microsoft.com/sharepoint/dev/declarative-customization/customize-default-site-design).

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:
Applicable: SharePoint Online
Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters

This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](https://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
