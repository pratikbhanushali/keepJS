# keepJS

Keep is a simple Javascript Library used to manage your Browser Storage. It uses Cookies, Local Storage and Session Storage for this purpose.

You can **SET**, **GET**, **DELETE** your data from browser storages.

**1. SET Data** - `keep.set()`

_Example :_   

`keep.set({ name : _"cookie-name"_, value: _"Hello World!"_, sess: _false_, expires: _"Mon, 4 Nov 2100 13:00:00 GMT"_, storage: _"C"_,  encrypt: _true_ });`

_Parameters:_   

**name** \ 		_Identifier used to store a value in browser storage._   
**value** \		_Value to be stored in the browser storage._     
**storage** \	_Optional: Defaults to Cookies. Possible values are  'C'(Cookies) / 'L'(localStorage) / 'S'(session storage)._        
**sess** \ 		_Optional: Defaults to true. Used to set cookie as session cookie or persistant cookie. Possible values are true / false._        
**expires** \	_Optional: Sets a cookie with an expiry. This key is used only when sess = true. Use the Javascript Date function to pass expiry E.g. ("Mon, 4 Nov 2100 13:00:00 GMT")_          
**path** \		_Optional: Defaults to '/'._        
**encrypt** \    _Optional: This key if set to boolean true, will encrypt data that goes into store._      

_P.S :_ **encrypt** - Do not SET this key to **true** if you want to use `cookie` data on the server-side.         


