#### Get Nearby Users’ Details Route:

API Path: api/users/getNearbyUsers?radius=${radius}

Method: GET

#### Description:
  - This is a protected route which gets the nearby users’ details after verifying JWT access token which is provided in the header.

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

    Name: nearbyUser

| Name          | Type    |
| ------------- |:------: |
| success       | boolean |
| message       | String  |
| data          | Object  |
