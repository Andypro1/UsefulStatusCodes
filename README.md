Proposed Status Code Extension to Hypertext Transfer Protocol -- HTTP/1.1, RFC 2616
=======================================================================

Communications are becoming increasingly shoehorned into the World Wide Web, and the notification at the core of this communication exists as a three digit code in HTTP called a status code.  This field is required for every HTTP response, and it may not be omitted.

Given that many packets traveling across the web today strive for terseness in order to maintain a good user experience, it seems silly that this crucial three digit code is not used to convey more information.  Hence, I propose to the W3C and web browser vendors this backwards compatible extension to the status codes defined in HTTP/1.1 for immediate implementation.

10.1 Informational 1xx
----------------------

10.2 Successful 2xx
-------------------

### 210 Hi
	
Servers may use this response when the first request is made from a particular client.  Recommended max use is once per 24 hour period, because it's redundant to say hello more than once per day.

### 211 Bye

When the client requests a resource that is known to be an end point of a process or for information, this response code may be used.  It offers an air of finality to the conversation.

### 212 Thank You

Web servers can be brutally cold and uncaring.  A polite server will use this response liberally when accepting something of value from the client.

### 213 You're Welcome

While servers are always in the business of serving, it stands to reason that sometimes, clients like to show appreciation for what they have been given.  This gives the server an opportunity to respond graciously with this status code.

### 214 Your Mom

This is a success code because, well, your mom.

10.3 Further Action Needed 3xx (formerly Redirection)
-----------------------------------------------------

	310 Afk Gone Home
	311 Also Afk.. Gone Home
	312 Afk Lunch
	314 Afk Bed
	315 Look Over There

10.4 Client Error 4xx
---------------------

	418 I'm A Teapot
	419 Lol
	422 I Blame You For That
	425 That Doesn't Logically Follow
	426 Can't Talk; Eating
	427 Game Cards Do Not Actually Talk
	428 Wat
	431 Off By 1
	432 Seriously You Were Off By 1 At 431

10.5 Server Error 5xx
---------------------

	537 I Like You A Lot But I Won't Be Sending You Any HTML

10.6 Server Commands 6xx (new)
------------------------

	601 No U