# API Doc
## Auth
<u>Getting QR Code</u>
 ``GET : /auth/getqr``
> Used to get a QR Code to Log into Whatsapp Web
	- If not logged in, returns a **QR Code**
	- If logged in, returns a "Authenticated" message.

## Chat
<u>Sending Messages</u>
``POST : /chat/sendmessage/<phone_number>``
> Request Body
> - message - contains the message to be sent
<hr>

<u>Get Chat By Id</u>
``GET : /chat/getchatbyid/<phone_number>``
>Returns a Chat

<hr>

<u>Get Chats</u>
``GET : /chat/getchats``
>Returns an Array of all Chats

## Contact
<u>Get Contacts</u>
``GET : /contact/getcontacts``
>Returns an Array of Contacts of the Current Instance

<hr>

<u>Get Contact</u>
``GET : /contact/getcontact/<phone_number>``
>Returns a Contact

<hr>

<u>Get Profile Pic</u>
``GET : /contact/getprofilepic/<phone_number>``
>Returns a URL of the User's Profile Picture if Privacy Settings allow it

<hr>

<u>Is Registered User</u>
``GET : /contact/isregistereduser/<phone_number>``
>Returns if a given User is registered on Whatsapp
