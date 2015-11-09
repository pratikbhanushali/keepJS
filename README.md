# keepJS
Keep is a simple Javascript Library used to manage your Browser Storage. It uses Cookies, Local Storage and Session Storage for this purpose.

You can #SET, #GET, #DELETE your data from browser storages.

Examples:

#1. #Setting data - #keep.set()

Parameters - 
 params
* 			@name 		Identifier used to store a value in browser storage.
* 			@value 		Value to be stored in the browser storage.
* 			@storage 	Optional: Defaults to Cookies. Possible values are  'C'(Cookies) / 'L'(localStorage) / 'S'(session storage).
* 			@sess 		Optional: Defaults to true. Used to set cookie as session cookie or persistant cookie. Possible values are true / false.
* 			@expires 	Optional: Sets a cookie with an expiry. This key is used only when @sess = true
* 			@path 		Optional: Defaults to '/'.
