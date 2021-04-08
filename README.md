# npm.mongo
npm.mongo mongodb wrapper for beginners.

![npm.mongo](https://nodei.co/npm/npm.mongo.png)

# Features
- Beginner friendly
- Easy to use
- Very similar to **[quick.db](https://npmjs.com/package/quick.db)**
- Dot notation support
- Import & export support
- Key value based
- Simple
- Asynchronous
- Multiple model support

```js
const { Database } = require("npm.mongo");
const db = new Database("mongodb://localhost/npm.mongo");

db.on("ready", () => {
    console.log("Database connected!");
});

await db.set("foo", "bar");

await db.get("foo");
```

# Example

```js
const { Database } = require("npm.mongo");
const db = new Database("mongodb://localhost/npm.mongo");

db.set("bayrak", { difficulty: "wen" }).then(console.log);

db.push("bayrak.xd", "wen").then(console.log);

db.add("bayrak.wen", 500).then(console.log);

db.push("bayrak.xd", "wen").then(console.log);

db.add("bayrak.wen", 500).then(console.log);

db.get("bayrak.wen").then(console.log);

db.get("bayrak.wen").then(console.log);

# OR

await db.set("bayrak", "wen");

await db.push("bayrak.xd", "wen");

await db.add("bayrak.wen", 500);

await db.push("bayrak.xd", "wen");

await db.add("bayrak.wen", 500);

await db.get("bayrak.wen");

await db.get("bayrak.wen");

```