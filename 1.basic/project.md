  - create a database named `sports`.

  //use sports

  - list all databases present in local mongod server.

  //show dbs

  - create 3 collections named `cricket`, `football`, `TT` in sports databse.

  db.cricket.insertMany([{name: "Bob", age: 24, email: 'bob@bob.com', cost:100}, {name: "Man", age: 21, email: 'man@man.com', cost: 500}, {name: "hi", age: 25, email: 'hi@hi.com', cost: 100}]), 
  db.football.insertMany([{name: "Bob", age: 
  24, email: 'bob@bob.com', cost:100}, {name: "Man", age: 21, email: 'man@man.com', cost: 500}, {name: "hi", age: 25, email: 'hi@hi.com', cost: 100}])

  db.TT.insertMany([{name: "Bob", age: 24, email: 'bob@bob.com', cost:100}, {name: "Man", age: 21, email: 'man@man.com', cost: 500}, {name: "hi", age: 25, email: 'hi@hi.com', cost: 100}]), 
  
  db.track.insertMany([{name: "Bob", age: 
  24, email: 'bob@bob.com', cost:100}, {name: "Man", age: 21, email: 'man@man.com', cost: 500}, {name: "hi", age: 25, email: 'hi@hi.com', cost: 100}])

  - add multiple players in those collections which should have fields like `name`, `age` and `email` and `cost`.
  - list all collections in sports database.

  //show collections

  - rename `TT` collection to `tennis`.

  //db.TT.renameCollection("Tennis")

  - create a capped collection called `khokho` which should have max 3 documents.
  Try inserting more than 3 and see what happens?

  //db.createCollection("khokho", {capped:true, size: 100000, max: 3000})

  db.khokho.insertMany([{name: "Bob", age: 24, email: 'bob@bob.com', cost:100}, {name: "Man", age: 21, email: 'man@man.com', cost: 500}, {name: "hi", age: 25, email: 'hi@hi.com', cost: 100}, {name: "hi", age: 25, email: 'hi@hi.co
m', cost: 100}])

  - check whether a collection is capped or not?

  //db.khokho.isCapped()

  - drop all documents from `football` collection.

  //db.football.remove({})

  - delete cricket collection completely.
  db.cricket.drop()

  - delete sports database. 
  use sports
  db.dropDatabase
