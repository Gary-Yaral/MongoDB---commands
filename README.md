# How to use MongoDB

**First One**
- Add MongoDB route to path of your computer
- Execute twice **CMD** like **administrator**
- Write this command in the first console
``` console
  mongod
```
- In the other console write the next command
``` console
  mongo
```

## Let's start to talk about the commands
Remember that you must write the commands in the second console

### Databases
**Show all databases**
``` console
  show dbs
```
**Create or switch database**
``` console
  use mydatabase
```

**Drop database**
``` console
  db.drop()
```
### Collections
**Add collections**
``` console
  db.myCollectionName
```
or
``` console
  db.createCollection('myCollectionName')
```

**Insert documents**
``` console
  db.myCollection.insert({name:"Claire",age:23})
```

**Update documents**
``` console
  db.myCollection.update({name:"Claire"},{$set:{age: 25}})
```

Increment a property
``` console
  db.myCollection.update({name:"Claire"},{$inc:{age: 2}})
```

Rename a property
``` console
  db.myCollection.update({name:"Claire"},{$rename:{age: "birthday"}})
```

