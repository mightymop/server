config value:

'jwtauthurl'=>'URL TO SERVICE WHICH TESTS THE JWT FOR VALIDITY'

This App will call the service with an HTTP Request and Authorization Header...

Authorization: Bearer <JSON-WEB-TOKEN-HERE>

The Service must respond with HTTP STATUSCODE 200, if the token is valid.
All other Statuscodes will prevent the user from login.
