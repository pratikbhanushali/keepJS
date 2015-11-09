# keepJS

Keep is a simple Javascript Library used to manage your Browser Storage. It uses Cookies, Local Storage and Session Storage for this purpose.

You can **SET**, **GET**, **DELETE** your data from browser storages.

**1. SET Data** - `keep.set()`

_Example :_   

`keep.set({ name : _"identifier-name"_, value: _"Hello World!"_, sess: _false_, expires: _"Mon, 4 Nov 2100 13:00:00 GMT"_, storage: _"C"_,  encrypt: _true_ });`

_Parameters:_   

**name**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_Identifier used to store a value in browser storage._   
**value**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_Value to be stored in the browser storage._     
**storage**&nbsp;&nbsp;&nbsp;_Optional: Defaults to Cookies. Possible values are  'C'(Cookies) / 'L'(localStorage) / 'S'(session storage)._        
**sess**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_Optional: Defaults to true. Used to set cookie as session cookie or persistant cookie. Possible values are true / false._        
**expires**&nbsp;&nbsp;&nbsp;_Optional: Sets a cookie with an expiry. This key is used only when sess = true. Use the Javascript Date function to pass expiry E.g. ("Mon, 4 Nov 2100 13:00:00 GMT")_          
**path**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_Optional: Defaults to '/'._        
**encrypt**&nbsp;&nbsp;&nbsp;_Optional: This key if set to boolean true, will encrypt data that goes into store._      

_P.S :_ **encrypt** - Do not SET this key to **true** if you want to use `cookie` data on the server-side.         
&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;
&nbsp;&nbsp;&nbsp;    

**1. GET Data** - `keep.set()`      

_Example :_     

`keep.get({ name : _"identifier-name"_ });`    

_Parameters:_   

**name**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_Identifier used to store a value in browser storage._   