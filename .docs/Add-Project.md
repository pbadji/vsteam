#include "./common/header.md"

# Add-Project

## SYNOPSIS
#include "./synopsis/Add-Project.md"

## SYNTAX

```
Add-Project [-Name] <String> [[-ProcessTemplate] <String>] [[-Description] <String>] [-TFVC]
```

## DESCRIPTION
This will create a new Team Project in your Team Services
account.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Add-Project 'MyProject'
```

This will add a project name MyProject with no description using the Scrum process
template and Git source control.

### -------------------------- EXAMPLE 2 --------------------------
```
Add-Project 'MyProject' -TFVC -ProcessTemplate Agile
```

This will add a project name MyProject with no description using the Agile process
template and TFVC source control.

## PARAMETERS

### -Name
The name of the project to create.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProcessTemplate
The name of the process template to use for the project.
The valid values are
Agile, Scrum or CMMI.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: Scrum
Accept pipeline input: False
Accept wildcard characters: False
```

### -Description
The description of the team project.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TFVC
Switches the source control from Git to TFVC.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-TeamAccount](Add-TeamAccount.md)
[Remove-Project](Remove-Project.md)
