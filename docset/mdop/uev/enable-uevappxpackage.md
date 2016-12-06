---
author: 
description: 
external help file: Microsoft.Uev.Commands.dll-Help.xml
keywords: powershell, cmdlet
manager: 
ms.assetid: BA8CF585-7F9E-4A13-91BC-FAB390E1AD00
ms.date: 2016-12-05
ms.devlang: powershell
ms.service: MDOP
ms.topic: reference
online version: 
schema: 2.0.0
title: Enable-UevAppxPackage
---

# Enable-UevAppxPackage

## SYNOPSIS
Enables uev_tla synchronization of Windows 8 apps.

## SYNTAX

### ParameterSetUser (Default)
```
Enable-UevAppxPackage [-CurrentComputerUser] [-PackageFamilyName] <String[]> [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### ParameterSetComputer
```
Enable-UevAppxPackage [-Computer] [-PackageFamilyName] <String[]> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Enable-UevAppxPackage** cmdlet enables uev_1 synchronization of Windows® 8 apps.
The cmdlet adds a setting to the computer or user sections of the registry that enables the package family names of Windows 8 apps that you specify.
If you do not specify the *Computer* or *CurrentComputerUser* parameters, the cmdlet enables the package family names for the current user.

## EXAMPLES

### Example 1: Enable synchronization of a Windows 8 app
```
PS C:\>Enable-UevAppxPackage -PackageFamilyName "Microsoft.BingTravel"
```

This command enables synchronization of settings for the Bing Travel Windows 8 app for the current user.

## PARAMETERS

### -Computer
Indicates that the cmdlet enables the package families that you specify for all users on the computer.

```yaml
Type: SwitchParameter
Parameter Sets: ParameterSetComputer
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -CurrentComputerUser
Indicates that the cmdlet enables the package families that you specify for all users on the computer.

```yaml
Type: SwitchParameter
Parameter Sets: ParameterSetUser
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PackageFamilyName
Specifies an array of names of package families.
The cmdlet enables the package families of Windows 8 apps that you specify.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Clear-UevAppxPackage](./Clear-UevAppxPackage.md)

[Disable-UevAppxPackage](./Disable-UevAppxPackage.md)

[Get-UevAppxPackage](./Get-UevAppxPackage.md)

