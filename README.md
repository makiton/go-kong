# go-kong #

go-kong is a Go client library for accessing Mashape's [Kong API](https://getkong.org/docs/0.9.x/admin-api/).

**Build Status:** [![Build Status](https://travis-ci.org/spicyusername/go-kong.svg?branch=master)](https://travis-ci.org/spicyusername/go-kong)  
**Test Coverage** [![Coverage Status](https://coveralls.io/repos/github/spicyusername/go-kong/badge.svg?branch=master)](https://coveralls.io/github/spicyusername/go-kong?branch=master)  

## Usage ##

```go
import "github.com/google/go-github/github"
```

Construct a new GitHub client, then use the various services on the client to
access different parts of the Kong API. For example:

```go
client := kong.NewClient(nil, "http://localhost:8001/")

// list all organizations for user "willnorris"
apis, _, err := client.Apis.Get("backend")
```