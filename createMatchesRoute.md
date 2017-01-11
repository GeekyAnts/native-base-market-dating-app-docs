#### Create Matches Route:

API Path: api/users/createMatches

Method: GET

#### Description:
  - This is a protected route which create matches using user and vote models in the database and return them.

#### Parameters:
  * Name: req

    Type: Object

  * Name: jwtAccessToken

    Type: String

    Inside: Header

    Description: JWT access token is used to check the authenticity of the user.

  * Name: res

    Type: Object

    Description: res is nothing but the response object which gets you the nearby users’ details.

    Http Code: 200

    Name: matchingUsers
    

| Name          | Type    |
| ------------- |:------: |
| success       | boolean |
| message       | String  |
| data          | Object  |
