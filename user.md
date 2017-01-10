File Name:  user.js
File Path:   /server/routes/user.js
Contains following routes:  
register, getNearbyUsers, saveVote and createMatches.
These functionalities are included in user Controller, getNearbyUsers Controller, saveVote Controller and match Controller respectively.

Registration Route:

API Path: api/users/register

Method: POST

Description:
-Register route is used to register a new user.
-This route also checks whether a user has already been registered or not; if not, the image of the profile pic of the user is stored on cloud using “Cloudinary” and the user is saved in the database.

Parameters:
Name: req
Type: Object
Name		Type
email		String
name		String
first_name	String
last_name	String
picture		Object
loc		Object
gender 	Number

Name: res
Type: Object
Response: Returns an object with three properties: success (bool), message, data.
The third parameter data is an object with two properties: jwtAccessToken and user object.
Http Code: 200
Name: returnObj
Type: Object
Name		Type
success	boolean
message	String
data		Object
