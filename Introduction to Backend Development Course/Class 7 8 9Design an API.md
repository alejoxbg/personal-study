As tweeter you have tweets, a message, to that message can added another messages as a comments, if we want to develop a clon of tweeter you need to create users, tweets, update users or messages, you can delete a user or a tweet, you have to see the users or the tweets,

Those are CRUD Create, Read, Update and Delete, everytime you need to use those verbs to use this that you can create by a API, if you build a API that can use the CRUDand you can connect it to the frontend you can have a application ready.

endpoint/route/path is a secction of a URL of our proyect 
![[Pasted image 20220723185710.png]]

Usually que use a /api/[something] as a endpoint


Lests start with the enpoints of the tweets

We have to follow the guides of CRUD (create, read, update, delete)

![[Pasted image 20220723191202.png]]


To the users and tweets you need models or tables in SQL, every data has a register, but when we program those models are called attributes.

Thoes variables are called parameters.

every time we enter those endpoints the server will respond with the info with a JSON format

![[Pasted image 20220723191748.png]]

```
GET) /api/tweets => shows all tweets
(POST) /api/post => publish a tweet
(GET) /api/tweets/:id => shows a single tweet
(UPDATE) /api/tweets/:id => updates a tweet
(DELETE) /api/tweets/:id => deletes a tweet

## Endpoints para Usuarios

(GET) /api/users => shows all users
(POST) /api/signup => registers an user
(GET) /api/users/:userID => shows an user
(UPDATE) /api/users/:userID => updates an user
(DELETE) /api/users/:userID => deletes an user
```