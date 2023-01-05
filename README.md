<h1 align="center">Polybase Collection Design</h1>

<p align="center">
	Polybase Collections Design Test Patterns for Building Various Applications.
</p>

## Main goals

- [ ] Use UID instead of public key to assign owner or creator.
- [ ] Add the ability to use multiple public keys for one account.

## Registration

```
user = Users.constructor( ... )

session = Sessions.constructor(user)
	-> user.auth()
```

## Create Post

```
session = Sessions.record( ... )

post = Posts.constructor(session, ... )
	-> session.auth()
```
