---
external help file: SMAzure_Compute.xml
online version: 322a1918-d734-42b4-bd0b-13d5ee8d37b5
schema: 2.0.0
updated_at: 9/28/2016 9:39 AM
ms.date: 9/28/2016
ms.topic: reference
source_repo: https://github.com/SummerSun/poc-azure-powershell.git
source_branch: master
gitcommit: https://github.com/SummerSun/poc-azure-powershell.git/blob/8903b0f1daa01932ac5fa167f377736de2df6709/azureps-cmdlets-docs/Service%20Management/Compute%20Cmdlets/v0.9.8/Get-AzureSchedulerJob.md
---

# Get-AzureSchedulerJob
## SYNOPSIS
Gets a list of scheduler jobs or a particular scheduler job.

## SYNTAX

```
Get-AzureSchedulerJob [-Location] <String> [-JobCollectionName] <String> [[-JobName] <String>]
 [[-JobState] <String>]
```

## DESCRIPTION
This topic describes the cmdlet in the 0.8.10 version of the Microsoft Azure PowerShell module.
To get the version of the module you're using, in the Azure PowerShell console, type (Get-Module -Name Azure).Version.

The Get-AzureSchedulerJobCollection cmdlet gets a list of scheduler jobs or a particular scheduler job.

## EXAMPLES

### Example 1: Get all jobs in a collection
```
PS C:\>Get-AzureSchedulerJob -Location "North Central US" -JobCollectionName "JobCollection01"
```

This command gets scheduler jobs that are part of the job collection named JobCollection01.

### Example 2: Get a named job
```
PS C:\>Get-AzureSchedulerJob -Location "North Central US" -JobCollectionName "JobCollection01" -JobName "Job01"
```

This command gets the job named Job01 from the collection named JobCollection01 in the specified location.

### Example 3: Get disabled jobs in a collection
```
PS C:\>Get-AzureSchedulerJobCollection -Location "North Central US" -JobCollectionName "JobCollection01" -JobState "Disabled"
```

This command gets all disabled scheduler jobs that are part of JobCollection01 in the specified location.

## PARAMETERS

### -JobCollectionName
Specifies the name of the collection that contains the scheduler job to get.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -JobName
Specifies the name of a scheduler job to get.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -JobState
Specifies the state of scheduler jobs to get.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 4
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Location
Specifies the name of the location that hosts the cloud service.
Valid values are: 

-- Anywhere Asia
-- Anywhere Europe
-- Anywhere US
-- East Asia
-- East US
-- North Central US
-- North Europe
-- South Central US
-- Southeast Asia
-- West Europe
-- West US

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Remove-AzureSchedulerJob](322a1918-d734-42b4-bd0b-13d5ee8d37b5)
