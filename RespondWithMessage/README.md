# Respond with message

Simple flow that is intended to make sure that a response message always has the same layout. This flow could be very useful for the creating of an API. By always using this, you make sure that the message always has the same layout

The response message can have the following four properties:

    {
	    "statusCode": 69,
	    "message": "hello world",
	    "stackTrace": "This is an error stack trace",
	    "httpCode": 418
	}
## Setting the parameters
You can either configure the properties via the properties of the subflow itself or by passing along via the msg.payload object. Items from the payload will always override the properties set on the subflow itself. 