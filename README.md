<h1 align="center">Polybase Collection Design</h1>

<p align="center">
	Polybase Collections Design Test Patterns for Building Various Applications.
</p>

## Main goals

- [ ] Use UID instead of public key to assign owner or creator.
- [ ] Add the ability to use multiple public keys for one account.
- [ ] Setting the level of access to each session.

## Registration

```
identity = Identity.constructor( ... )

session = Session.constructor(account)
	-> account.auth()
```

## Create Post

```
session = Session.record( ... )

post = Post.constructor(session, ... )
	-> session.auth()
```
