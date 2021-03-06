﻿```PowerShell

NAME
    Get-UiPathAuthToken
    
SYNOPSIS
    Obtains an UiPath authentication token
    
    
SYNTAX
    Get-UiPathAuthToken [-URL] <string> -Password <string> -Username <string> [-Session <SwitchParameter>] 
    [-TenantName <string>] [<CommonParameters>]
    
    Get-UiPathAuthToken [-URL] <string> -WindowsCredentials <SwitchParameter> [-Session <SwitchParameter>] 
    [-TenantName <string>] [<CommonParameters>]
    
    Get-UiPathAuthToken [-URL] <string> -Unauthenticated <SwitchParameter> [-Session <SwitchParameter>] [-TenantName 
    <string>] [<CommonParameters>]
    
    
DESCRIPTION
    The authentication token is needed for other UiPath Powershell cmdlets.
    

PARAMETERS
    -URL <string>
        
        Required?                    true
        Position?                    0
        Default value                
        Accept pipeline input?       false
        Accept wildcard characters?  false
        
    -TenantName <string>
        
        Required?                    false
        Position?                    named
        Default value                
        Accept pipeline input?       false
        Accept wildcard characters?  false
        
    -Username <string>
        
        Required?                    true
        Position?                    named
        Default value                
        Accept pipeline input?       false
        Accept wildcard characters?  false
        
    -Password <string>
        
        Required?                    true
        Position?                    named
        Default value                
        Accept pipeline input?       false
        Accept wildcard characters?  false
        
    -WindowsCredentials <SwitchParameter>
        
        Required?                    true
        Position?                    named
        Default value                False
        Accept pipeline input?       false
        Accept wildcard characters?  false
        
    -Unauthenticated <SwitchParameter>
        
        Required?                    true
        Position?                    named
        Default value                False
        Accept pipeline input?       false
        Accept wildcard characters?  false
        
    -Session <SwitchParameter>
        
        Required?                    false
        Position?                    named
        Default value                False
        Accept pipeline input?       false
        Accept wildcard characters?  false
        
    <CommonParameters>
        This cmdlet supports the common parameters: Verbose, Debug,
        ErrorAction, ErrorVariable, WarningAction, WarningVariable,
        OutBuffer, PipelineVariable, and OutVariable. For more information, see 
        about_CommonParameters (https:/go.microsoft.com/fwlink/?LinkID=113216). 
    
INPUTS
    
OUTPUTS
    
    ----------  EXAMPLE 1  ----------
    
    Get-UiPathAuthToken -URL https://platform.uipath.com -Username <myuser> -Password <mypassword>
    
    Connect to UiPath public platform Orchestrator, using user name and password.
    ----------  EXAMPLE 2  ----------
    
    Get-UiPathAuthToken -URL https://platform.uipath.com -Username <myuser> -Password <mypassword> -Session
    
    Connect to UiPath public platform Orchestrator, using user name and password and save the token for the current 
    session.
    ----------  EXAMPLE 3  ----------
    
    Get-UiPathAuthToken -URL https://uipath.corpnet -WindowsCredentials -Session
    
    Connect to a private Orchestrator with Windows enabled, using current Windows credentials and save the token for 
    current session.
    
RELATED LINKS



```
