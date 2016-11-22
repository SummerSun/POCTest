---
external help file: Microsoft.Azure.SqlDatabase.Jobs.PowerShell.dll-Help.xml
online version:
schema: 2.0.0
ms.assetid: 684FC100-2F64-43BC-9F78-47711EE4B685
updated_at: 11/17/2016 5:33 AM
ms.date: 11/17/2016
content_git_url: https://github.com/SummerSun/azure-docs-powershell-int/blob/master/azureps-cmdlets-docs/ElasticDatabaseJobs/v0.8.33/Remove-AzureSqlJobTrigger.md
gitcommit: https://github.com/SummerSun/azure-docs-powershell-int/blob/2692a7998846b66d06a416c56978167da402f8d5/azureps-cmdlets-docs/ElasticDatabaseJobs/v0.8.33/Remove-AzureSqlJobTrigger.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureSqlJobTrigger

## SYNOPSIS
Removes a job trigger to stop future jobs runs according to a schedule.

## SYNTAX

```
Remove-AzureSqlJobTrigger -JobName <String> -ScheduleName <String>
 [[-AzureSqlJobConnection] <AzureSqlJobConnection>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureSqlJobTrigger** cmdlet removes a job trigger to stop future job runs according to a schedule.

## EXAMPLES

### Example 1: Remove a job trigger by job and schedule name
```
PS C:\>Remove-AzureSqlJobTrigger -JobName "MyJob" -ScheduleName "MyOneMinuteIntervalSchedule"
```

This command removes the job trigger specified by job name and schedule name.

## PARAMETERS

### -AzureSqlJobConnection
Specifies the connection state object for the job.
You can get the connection state object through the [New-AzureSqlJobConnection](./New-AzureSqlJobConnection.md) cmdlet.
If you do not specify this parameter, the connection state is used from a prior call to the [Use-AzureSqlJobConnection](./Use-AzureSqlJobConnection.md) cmdlet.

```yaml
Type: AzureSqlJobConnection
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -JobName
Specifies the name of the job within the job trigger.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ScheduleName
Specifies the name of the schedule within the job trigger.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
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

[Get-AzureSqlJobTrigger](xref:ElasticDatabaseJobs/v0.8.33/Get-AzureSqlJobTrigger.md)

[New-AzureSqlJobTrigger](xref:ElasticDatabaseJobs/v0.8.33/New-AzureSqlJobTrigger.md)

[Remove-AzureSqlJobTrigger](xref:ElasticDatabaseJobs/v0.8.33/Remove-AzureSqlJobTrigger.md)