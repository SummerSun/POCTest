---
external help file: SMAzure_Compute.xml
online version: 07ab8d50-c6de-45f1-8576-99b76f798bca
schema: 2.0.0
updated_at: 9/28/2016 9:39 AM
ms.date: 9/28/2016
ms.topic: reference
source_repo: https://github.com/SummerSun/poc-azure-powershell.git
source_branch: master
gitcommit: https://github.com/SummerSun/poc-azure-powershell.git/blob/8903b0f1daa01932ac5fa167f377736de2df6709/azureps-cmdlets-docs/Service%20Management/Compute%20Cmdlets/v0.9.8/New-AzureSBAuthorizationRule.md
---

# New-AzureSBAuthorizationRule
## SYNOPSIS
Creates new Service Bus authorization rule

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
New-AzureSBAuthorizationRule [-Name] <String> [-Permission] [-Namespace] <String> [-EntityName] <String>
 [-EntityType] <ServiceBusEntityType> [[-PrimaryKey] <String>] [[-SecondaryKey] <String>]
```

### UNNAMED_PARAMETER_SET_2
```
New-AzureSBAuthorizationRule [-Name] <String> [-Permission] [-Namespace] <String> [[-PrimaryKey] <String>]
 [[-SecondaryKey] <String>]
```

## DESCRIPTION
Creates new Service Bus authorization rule

## EXAMPLES

### -------------- Creates new authorization rule with generated primary key --------------
```
C:\PS>New-AzureSBAuthorizationRule -Name MyRule -Namespace MyNamespace -Permission $("Send")
```

Creates new authorization rule on namespace level with Send permission

### -------------- Creates new authorization rule providing primary key --------------
```
C:\PS>New-AzureSBAuthorizationRule -Name MyRule -Namespace MyNamespace -Permission $("Manage", "Listen", "Send") -EntityName MyEntity -EntityType Queue -PrimaryKey P+lL/Mnd2Z9sj5hwMrRyAxQDdX8RHfbdqU2eIAqs1rc=
```

Creates new authorization rule on MyEntity Queue level with all permissions

## PARAMETERS

### -EntityName
The entity name to apply rule at.

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: 4
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -EntityType
The entity type (Queue, Topic, Relay, NotificationHub).

```yaml
Type: ServiceBusEntityType
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: 5
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
The unique authorization rule name

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -Namespace
The namespace name to apply the authorization rule.
If no EntityName provided the rule will be on the namespace level

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Permission
The authorization permissions (Send, Manage, Listen)

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 
Accepted values: Manage, Send, Listen

Required: False
Position: 2
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -PrimaryKey
The Shared Access Signature primary key.
Will be generated if not provided

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 6
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

### -SecondaryKey
The Shared Access Signature secondary key

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 7
Default value: 
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureSBAuthorizationRule](07ab8d50-c6de-45f1-8576-99b76f798bca)

[Remove-AzureSBAuthorizationRule](7d4951b1-15ff-4fa4-9122-36538eee9cbe)

[Set-AzureSBAuthorizationRule](c199f0d5-8f84-4106-ac4b-afc2192d1218)
