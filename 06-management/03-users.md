---
pageTitle: Managing Users
keywords: typedb, management, authentication, users
longTailKeywords: typedb managing users, typedb authentication, typedb users
Summary: User authentication in TypeDB Cluster.
toc: false
---

## Managing Users [TypeDB Cluster ONLY]
The ability to manage users and authenticate their access to [databases](../06-management/01-database.md) is limited to TypeDB Cluster and is not available in TypeDB.

In order to manage users, we first need to enter the TypeDB Console. To connect to TypeDB Cluster with TypeDB Console,
You'll need to specify that you're connecting to TypeDB Cluster and provide a username and password:
```
./typedb console --cluster=<address> --username=<username> --password=<password>
```

Then, we can use the following commands to manage users:

### Retrieve all users
```
user list
```

### Create a new user
```
user create <username> <password>
```

### Delete a user
```
user delete <username>
```

### Reset password of user
```
user password <username>
```