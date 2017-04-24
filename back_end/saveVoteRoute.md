#### Save Vote Route:

API Path: api/users/saveVote

Method: POST

#### Description:
  - This is a protected route which saves the vote in database.

#### Parameters:
  * Name: req

    Type: Object

| Name          | Type   |
| ------------- |:------:|
| targetId      | String |
| target        | String |
| isLiked       | String |

  * Name: jwtAccessToken

    Type: String

    Inside: Header

    Description: JWT access token is used to check the authenticity of the user.

  * Name: res

    Type: Object

    Http Code: 200
    
    Name: returnObj

| Name          | Type    |
| ------------- |:------: |
| success       | boolean |
| message       | String  |
| data          | Object  |
