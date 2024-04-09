# Handle error

Simple flow that is intended to make sure that errors are caught, and a response message that always has the same layout will be created. This flow could be very useful for the creating of an API. By always using this, you make sure that the error message always has the same layout

The response message can have the following four properties:
   {
	    "statusCode": 3,
	    "message": "An unexpected error occurred",
	    "stackTrace": "TypeError: Cannot read properties of null (reading 'payload')",
	    "httpCode": 500
	}
	
## Setting the parameters
Via the setting properties of the subflow itself, it's possible to set the following properties
### ErrorCode
If the error code is filled in this will be used, otherwise **0** will be used.

### Message
If the message is filled in this will be used, otherwise **An unexpected error occurred** will be used.

### OutputStackTrace
If OutputStackTrace is set to true the stack trace will be added to the message, otherwise it will be kept internal