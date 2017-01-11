#### Logout Route:

###### API Path: api/auth/logout

###### Method: GET

#### Description:
  - ###### This is a protected route which requires authentication token in the header. Logout route simply changes the login status and logouts the user from the database.

#### Parameters:
  * ###### Name: jwtAccessToken
    ###### Type: String
    ###### Inside: Header
    ###### Description: JWT access token is used to check the authenticity of the user.

  * ###### Name: res
    ###### Type: Object
    ###### Description: res is nothing but the response object which gets you the nearby users’ details.
    ###### Http Code: 200
    ###### Name: matchingUsers

| Name          | Type    |
| ------------- |:------: |
| success       | boolean |
| message       | String  |
| data          | Object  |
