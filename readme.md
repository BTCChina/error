```
                          _     __                                    
  _______  ______ _____  (_)___/ /__        ___  ______________  _____
 / ___/ / / / __ `/ __ \/ / __  / _ \______/ _ \/ ___/ ___/ __ \/ ___/
/ /__/ /_/ / /_/ / / / / / /_/ /  __/_____/  __/ /  / /  / /_/ / /    
\___/\__, /\__,_/_/ /_/_/\__,_/\___/      \___/_/  /_/   \____/_/     
    /____/                                                            
```
# Cyanide Error
Genine Error Thrower, which:
- Throws errors according to policies.
- Logs errors when throwing errors
- Separates Enduser / Debugger error Description

### Error Configuration
__Configuration for single error looks like this:__

```javascript
"header_policy_error": {      							// Error Name        
	"policy": "header_policy",							// Policy Name
	"log_path":"validator",								// Plcae to log the Error
	"log_root":"",										// Root of the Log
	"http_status": 401,									// http_status if needed
	"code": "0002",										// Error Code
	"msg": "request header did not contain credential", // Error Message
	"emitter": "request"								// Source Of Error
}
```