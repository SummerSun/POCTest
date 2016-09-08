---
external help file: RMAzure_Automation.xml
online version: 091cd841-4aaf-45de-a8f2-6f973fb9c91b
schema: 2.0.0
updated_at: 9/8/2016 10:32 AM
ms.date: 9/8/2016
ms.topic: reference
content_git_url: https://github.com/azure/azure-docs-powershell.git/blob/master/azureps-cmdlets-docs/Resource%20Manager/Automation%20Cmdlets/v0.9.8/Get-AzureRmAutomationDscConfiguration.md
original_content_git_url: https://github.com/azure/azure-docs-powershell.git/blob/master/azureps-cmdlets-docs/Resource%20Manager/Automation%20Cmdlets/v0.9.8/Get-AzureRmAutomationDscConfiguration.md
gitcommit: https://github.com/azure/azure-docs-powershell.git/blob/8903b0f1daa01932ac5fa167f377736de2df6709/azureps-cmdlets-docs/Resource%20Manager/Automation%20Cmdlets/v0.9.8/Get-AzureRmAutomationDscConfiguration.md
---

# Get-AzureRmAutomationDscConfiguration
## SYNOPSIS
Gets DSC configurations from Automation.

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Get-AzureRmAutomationDscConfiguration [-ResourceGroupName] <String> [-AutomationAccountName] <String>
```

### UNNAMED_PARAMETER_SET_2
```
Get-AzureRmAutomationDscConfiguration [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [-Name] <String>
```

## DESCRIPTION
The **Get-AzureRmAutomationDscConfiguration** cmdlet gets APS Desired State Configuration (DSC) configurations from azure_2 Automation.

## EXAMPLES

### Example 1: Get all DSC configurations
```
PS C:\>Get-AzureRmAutomationDscConfiguration -ResourceGroupName "ResourceGroup03" -AutomationAccountName "Contoso17"
```

This command gets metadata for all DSC configurations in the Automation account named Contoso17.

### Example 2: Get a DSC configuration by name
```
PS C:\>Get-AzureRmAutomationDscConfiguration -ResourceGroupName "ResourceGroup03" -AutomationAccountName "Contoso17" -Name "ContosoConfiguration"
```

This command gets metadata for a DSC configuration named MyConfiguration in the Automation account named Contoso17.

## PARAMETERS

### -AutomationAccountName
Specifies the name of the Automation account that contains DSC configurations that this cmdlet gets.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of the DSC configuration that this cmdlet gets.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: ConfigurationName

Required: True
Position: 3
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of a resource group for which this cmdlet gets DSC configurations.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Export-AzureRmAutomationDscConfiguration](091cd841-4aaf-45de-a8f2-6f973fb9c91b)

[Import-AzureRmAutomationDscConfiguration](9e316628-0101-4da8-8a9f-843f8442e52d)
