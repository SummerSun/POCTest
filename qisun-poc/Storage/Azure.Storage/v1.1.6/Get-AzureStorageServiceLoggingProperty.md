---
external help file: Microsoft.WindowsAzure.Commands.Storage.dll-Help.xml
online version: .\New-AzureStorageContext.md
schema: 2.0.0
ms.assetid: 02217F39-6C93-401B-8801-52FDD38BA751
updated_at: 10/19/2016 3:33 AM
ms.date: 10/19/2016
content_git_url: https://github.com/SummerSun/azure-docs-powershell-int/blob/master/azureps-cmdlets-docs/Storage/Azure.Storage/v1.1.6/Get-AzureStorageServiceLoggingProperty.md
original_content_git_url: https://github.com/SummerSun/azure-docs-powershell-int/blob/master/azureps-cmdlets-docs/Storage/Azure.Storage/v1.1.6/Get-AzureStorageServiceLoggingProperty.md
gitcommit: https://github.com/SummerSun/azure-docs-powershell-int/blob/c0d1e448da01261236e9ece01ca5c2a98effbf31/azureps-cmdlets-docs/Storage/Azure.Storage/v1.1.6/Get-AzureStorageServiceLoggingProperty.md
ms.topic: reference
ms.prod: powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
open_to_public_contributors: True
ms.service: Storage
---

# Get-AzureStorageServiceLoggingProperty

## SYNOPSIS
Gets logging properties for azure_2 Storage services.

## SYNTAX

```
Get-AzureStorageServiceLoggingProperty [-ServiceType] <StorageServiceType> [-Context <AzureStorageContext>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-PipelineVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureStorageServiceLoggingProperty** cmdlet gets logging properties for azure_2 Storage services.

## EXAMPLES

### Example 1: Get logging properties for the Blob service
```
C:\PS>Get-AzureStorageServiceLoggingProperty -ServiceType Blob
```

This command gets logging properties for blob storage.

## PARAMETERS

### -ServiceType
Specifies the storage service type.
This cmdlet gets the logging properties for the service type that this parameter specifies.
psdx_paramvalues

- Blob 
- Table
- Queue
- File

The value of File is not currently supported.

```yaml
Type: StorageServiceType
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Context
Specifies an azure_2 storage context.
To obtain a storage context, use the New-AzureStorageContext cmdlet.

```yaml
Type: AzureStorageContext
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -InformationAction
@{Text=}```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
@{Text=}```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PipelineVariable
@{Text=}```yaml
Type: String
Parameter Sets: (All)
Aliases: pv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[New-AzureStorageContext](xref:Storage/Azure.Storage/v1.1.6/New-AzureStorageContext.md)

[Set-AzureStorageServiceLoggingProperty](xref:Storage/Azure.Storage/v1.1.6/Set-AzureStorageServiceLoggingProperty.md)


