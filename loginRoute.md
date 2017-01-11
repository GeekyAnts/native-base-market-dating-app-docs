#### Login Route:

###### API Path: api/auth/login

###### Method: POST

#### Description:
  - ###### Login route verifies email of the user. Once a user is authenticated, a token is generated.
  - ###### Also, it updates the user details, such as location etc.

#### Parameters:
  * ###### Name: req
    ###### Type: Object

| Name       | In       | Type    |
| ---------- |:--------:| ------: |
| user       | req.body | Object  |

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
