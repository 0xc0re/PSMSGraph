# Get-AADUserAppRoleAssignment

## SYNOPSIS
Returns the App Role Assigmnets for the given user

## SYNTAX

```
Get-AADUserAppRoleAssignment [-User] <Object[]> [[-BaseUrl] <String>] [[-APIVersion] <String>] [-WhatIf]
 [-Confirm]
```

## DESCRIPTION
Returns the App Role Assigmnets for the given user.
This can be used to see what applications to which Azure AD SaaS Applications (Service Principals) the user has been assigned access.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
$AADAppAssignments = $AADUser | Get-AADUserAppRoleAssignment
```

## PARAMETERS

### -User
A MSGraphAPI.DirectoryObject.User object retruned by Get-AADUser* cmdlets

```yaml
Type: Object[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -BaseUrl
The Azure AD Graph Base URL.
This is not required.
Deafult 
    https://graph.windows.net

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: Https://graph.windows.net
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -APIVersion
version og the API to use.
Default is 1.6

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: 1.6
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

### MSGraphAPI.DirectoryObject.AppRoleAssignment

## NOTES
Additional information about the function.

## RELATED LINKS

[http://psmsgraph.readthedocs.io/en/latest/functions/Get-AADUserAppRoleAssignment](http://psmsgraph.readthedocs.io/en/latest/functions/Get-AADUserAppRoleAssignment)

