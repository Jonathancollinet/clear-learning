# Les erreurs

---------------------------
*Error code indicating some error other than those enumerated here.
@constant*

***OTHER_CAUSE: -1***

---------------------------
*Error code indicating that something has gone wrong with the server.
If you get this error code, it is Parse's fault. Contact us at
https://parse.com/help
@constant*

***INTERNAL_SERVER_ERROR: 1***

---------------------------
*Error code indicating the connection to the Parse servers failed.
@constant*

***CONNECTION_FAILED: 100***

---------------------------
*Error code indicating the specified object doesn't exist.
@constant*

***OBJECT_NOT_FOUND: 101***

---------------------------
*Error code indicating you tried to query with a datatype that doesn't
support it, like exact matching an array or object.
@constant*

***INVALID_QUERY: 102***

---------------------------
*Error code indicating a missing or invalid classname. Classnames are
case-sensitive. They must start with a letter, and a-zA-Z0-9_ are the
only valid characters.
@constant*

***INVALID_CLASS_NAME: 103***

---------------------------
*Error code indicating an unspecified object id.
@constant*

***MISSING_OBJECT_ID: 104***

---------------------------
*Error code indicating an invalid key name. Keys are case-sensitive. They
must start with a letter, and a-zA-Z0-9_ are the only valid characters.
@constant*

***INVALID_KEY_NAME: 105***

---------------------------
*Error code indicating a malformed pointer. You should not see this unless
you have been mucking about changing internal Parse code.
@constant*

***INVALID_POINTER: 106***

---------------------------
*Error code indicating that badly formed JSON was received upstream. This
either indicates you have done something unusual with modifying how
things encode to JSON, or the network is failing badly.
@constant*

***INVALID_JSON: 107***

---------------------------
*Error code indicating that the feature you tried to access is only
available internally for testing purposes.
@constant*

***COMMAND_UNAVAILABLE: 108***

---------------------------
*You must call Parse.initialize before using the Parse library.
@constant*

***NOT_INITIALIZED: 109***

---------------------------
*Error code indicating that a field was set to an inconsistent type.
@constant*

***INCORRECT_TYPE: 111***

---------------------------
*Error code indicating an invalid channel name. A channel name is either
an empty string (the broadcast channel) or contains only a-zA-Z0-9_
characters and starts with a letter.
@constant*

***INVALID_CHANNEL_NAME: 112***

---------------------------
*Error code indicating that push is misconfigured.
@constant*

***PUSH_MISCONFIGURED: 115***

---------------------------
*Error code indicating that the object is too large.
@constant*

***OBJECT_TOO_LARGE: 116***

---------------------------
*Error code indicating that the operation isn't allowed for clients.
@constant*

***OPERATION_FORBIDDEN: 119***

---------------------------
*Error code indicating the result was not found in the cache.
@constant*

***CACHE_MISS: 120***

---------------------------
*Error code indicating that an invalid key was used in a nested
JSONObject.
@constant*

***INVALID_NESTED_KEY: 121***

---------------------------
*Error code indicating that an invalid filename was used for ParseFile.
A valid file name contains only a-zA-Z0-9_. characters and is between 1
and 128 characters.
@constant*

***INVALID_FILE_NAME: 122***

---------------------------
*Error code indicating an invalid ACL was provided.
@constant*

***INVALID_ACL: 123***

---------------------------
*Error code indicating that the request timed out on the server. Typically
this indicates that the request is too expensive to run.
@constant*

***TIMEOUT: 124***

---------------------------
*Error code indicating that the email address was invalid.
@constant*

***INVALID_EMAIL_ADDRESS: 125***

---------------------------
*Error code indicating a missing content type.
@constant*

***MISSING_CONTENT_TYPE: 126***

---------------------------
*Error code indicating a missing content length.
@constant*

***MISSING_CONTENT_LENGTH: 127***

---------------------------
*Error code indicating an invalid content length.
@constant*

***INVALID_CONTENT_LENGTH: 128***

---------------------------
*Error code indicating a file that was too large.
@constant*

***FILE_TOO_LARGE: 129***

---------------------------
*Error code indicating an error saving a file.
@constant*

***FILE_SAVE_ERROR: 130***

---------------------------
*Error code indicating that a unique field was given a value that is
already taken.
@constant*

***DUPLICATE_VALUE: 137***

---------------------------
*Error code indicating that a role's name is invalid.
@constant*

***INVALID_ROLE_NAME: 139***

---------------------------
*Error code indicating that an application quota was exceeded.  Upgrade to
resolve.
@constant*

***EXCEEDED_QUOTA: 140***

---------------------------
*Error code indicating that a Cloud Code script failed.
@constant*

***SCRIPT_FAILED: 141***

---------------------------
*Error code indicating that a Cloud Code validation failed.
@constant*

***VALIDATION_ERROR: 142***

---------------------------
*Error code indicating that invalid image data was provided.
@constant*

***INVALID_IMAGE_DATA: 150***

---------------------------
*Error code indicating an unsaved file.
@constant*

***UNSAVED_FILE_ERROR: 151***

---------------------------
*Error code indicating an invalid push time.*

***INVALID_PUSH_TIME_ERROR: 152***

---------------------------
*Error code indicating an error deleting a file.
@constant*

***FILE_DELETE_ERROR: 153***

---------------------------
*Error code indicating that the application has exceeded its request
limit.
@constant*

***REQUEST_LIMIT_EXCEEDED: 155***

---------------------------
*Error code indicating an invalid event name.*

***INVALID_EVENT_NAME: 160***

---------------------------
*Error code indicating that the username is missing or empty.
@constant*

***USERNAME_MISSING: 200***

---------------------------
*Error code indicating that the password is missing or empty.
@constant*

***PASSWORD_MISSING: 201***

---------------------------
*Error code indicating that the username has already been taken.
@constant*

***USERNAME_TAKEN: 202***

---------------------------
*Error code indicating that the email has already been taken.
@constant*

***EMAIL_TAKEN: 203***

---------------------------
*Error code indicating that the email is missing, but must be specified.
@constant*

***EMAIL_MISSING: 204***

---------------------------
*Error code indicating that a user with the specified email was not found.
@constant*

***EMAIL_NOT_FOUND: 205***

---------------------------
*Error code indicating that a user object without a valid session could
not be altered.
@constant*

***SESSION_MISSING: 206***

---------------------------
*Error code indicating that a user can only be created through signup.
@constant*

***MUST_CREATE_USER_THROUGH_SIGNUP: 207***

---------------------------
*Error code indicating that an an account being linked is already linked
to another user.
@constant*

***ACCOUNT_ALREADY_LINKED: 208***

---------------------------
*Error code indicating that the current session token is invalid.
@constant*

***INVALID_SESSION_TOKEN: 209***

---------------------------
*Error code indicating that a user cannot be linked to an account because
that account's id could not be found.
@constant*

***LINKED_ID_MISSING: 250***

---------------------------
*Error code indicating that a user with a linked (e.g. Facebook) account
has an invalid session.
@constant*

***INVALID_LINKED_SESSION: 251***

---------------------------
*Error code indicating that a service being linked (e.g. Facebook or
Twitter) is unsupported.
@constant*

***UNSUPPORTED_SERVICE: 252***

---------------------------
*Error code indicating that there were multiple errors. Aggregate errors
have an "errors" property, which is an array of error objects with more
detail about each error that occurred.
@constant*

***AGGREGATE_ERROR: 600***

---------------------------
*Error code indicating the client was unable to read an input file.
@constant*

***FILE_READ_ERROR: 601***

---------------------------
*Error code indicating a real error code is unavailable because
we had to use an XDomainRequest object to allow CORS requests in
Internet Explorer, which strips the body from HTTP responses that have
a non-2XX status code.
@constant*

***X_DOMAIN_REQUEST: 602***

---------------------------
