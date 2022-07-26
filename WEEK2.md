# Week 2: Express, Async/Await, Databases (PostgreSQL), ORMs (Sequelize)

[⬅ Go Back](README.md)

## Day 1: Holiday!

## Day 2: Express, Intro to DB and SQL

- Pre-Work:
  - [📺 Web Dev Simplified: What is an API?][what-is-an-api]
  - [📺 Codecademy: Back-End Web Architecture][codecademy-be-web-arch]
  - 📤 Download an API development tool (your choice) 📥
    - [Postman](https://www.postman.com/)
    - [Insomnia](https://insomnia.rest/)
  - [📖 Schema Design Overview][schema-design]

[schema-design]: https://medium.com/@kimtnguyen/relational-database-schema-design-overview-70e447ff66f9
[what-is-an-api]: https://youtu.be/tgbRY96q-KM
[codecademy-be-web-arch]: https://www.codecademy.com/articles/back-end-architecture
[twilio-async-await]: https://www.twilio.com/blog/2015/10/asyncawait-the-hero-javascript-deserved.html

| Topic                           | Lecture               | Slides                   | Demo                   | Solution                   | Review                     |
| ------------------------------- | --------------------- | ------------------------ | ---------------------- | -------------------------- | -------------------------- |
| Express 201 (Wizard News Pt 1)  | | [🖼️][express-201-slides] | |  |  |
| Intro to Databases & PostgreSQL | -                     | [🖼️][db-slides]          | -                      | -                          | -                          |
| Intro to SQL                    |        | [🖼️][sql-slides]         |         | -                          | -                          |
| Morning Review                  |      | [🎟][am-rev-2-1-ticket]   |  |       | -                          |

[//]: # ' Paste in table above >> [📺][express-201-lec] '
[express-201-lec]: https://youtu.be/Mg6O-1um10w
[express-201-slides]: https://docs.google.com/presentation/d/1cS548bLr3YMkA9tdwviIzwVU-qO29uOuw_DSJoD4O1o/edit?usp=sharing
[//]: # ' Paste in table above >> [🧑‍💻][express-201-demo] '
[express-201-demo]: 01-junior-phase/day-6-express-sql/express201
[//]: # ' Paste in table above >> [👾][express-wizard-1-sol] '
[express-wizard-1-sol]: https://github.com/FullstackAcademy/Solution.Wizard-news/tree/Part1
[//]: # ' Paste in table above >> [📺][express-wizard-1-rev] '
[express-wizard-1-rev]: https://www.youtube.com/watch?v=w07G_eMRFZ4
[//]: # ' Paste in table above >> [🖼️][db-slides] '
[db-slides]: https://docs.google.com/presentation/d/13VsDAKOCCJulTYtWSbg0gyDX4sqMRWaNVphE0okLmPM
[//]: # ' Paste in table above >> [🖼️][sql-slides] '
[sql-slides]: https://docs.google.com/presentation/d/1Wu-rfuuJ73MZfKX--mTdVXoYmOMFcd19ay-fvQuWAA4
[//]: # ' Paste in table above >> [📺][sql-lec] '
[sql-lec]: https://youtu.be/plKBZjg_2xw
[sql-slides]: https://docs.google.com/presentation/d/1Wu-rfuuJ73MZfKX--mTdVXoYmOMFcd19ay-fvQuWAA4/edit?usp=sharing
[//]: # ' Paste in table above >> [🧑‍💻][sql-demo] '
[sql-demo]: 01-junior-phase/day-6-express-sql/intro-sql
[//]: # ' Paste in table above >> [📺][am-rev-2-1] '
[am-rev-2-1]: https://youtu.be/RUZp09FkLUs
[//]: # ' Paste in table above >> [🎟][am-rev-2-1-ticket] '
[am-rev-2-1-ticket]: https://forms.gle/SwAmJ6bae7BcApoi8
[//]: # ' Paste in table above >> [🧑‍💻][am-rev-2-1-demo] '
[am-rev-2-1-demo]: 01-junior-phase/day-6-express-sql/morning-review
[//]: # ' Paste in table above >> [👾][am-rev-2-1-sol] '
[am-rev-2-1-sol]: https://github.com/FullstackAcademy/2206-FSA-RM-WEB-FT/blob/main/01-junior-phase/exit-ticket-solutions/06-sql.md

- **You should be able to:**
  - Describe the role of a client, a server, and HTTP
  - Describe Express middleware, requests, and responses
  - Handle URL params in an Express route
  - Know when and why you would use `app.use` and `next` in your Express app
  - Use `module.exports` and `require` to create modular applications
  - Handle asynchronous code and Promises with `async`/`await`

**<details><summary>📎 Extra Resources EXPRESS :</summary>**

- [📖 A Simple Explanation of Express Middleware][express-middleware]
- [📖 Nodejs in Flames][nodejs-flames]

[express-middleware]: https://medium.com/@agoiabeladeyemi/a-simple-explanation-of-express-middleware-c68ea839f498
[nodejs-flames]: https://medium.com/netflix-techblog/node-js-in-flames-ddd073803aa4

- **You should be able to:**
  - Explain what a database is, and why you would use one
  - Write SQL queries using some common keywords (`SELECT`, `FROM`, `WHERE`, `ORDER BY`, `JOIN`, etc)
  - Articulate what a primary key is
  - Articulate what a foreign key is, and why you would use one
  - Explain the differences between a 1-to-1, 1-to-many, and many-to-many relationship

</details>

**<details><summary>📎 Extra Resources SQL:</summary>**

- [Normalization][normalization]
- [SQL-Relationships][sql-relationships]
- [SQLzoo][sql-zoo]
- [SQL vs NoSQL][sql-nosql]
- [📖 SQL W3schools][sql-w3]
- [📖 What is a RDBMS anyway?][rdbms-what]

[normalization]: https://opentextbc.ca/dbdesign01/chapter/chapter-12-normalization/
[sql-relationships]: https://code.tutsplus.com/articles/sql-for-beginners-part-3-database-relationships--net-8561
[sql-zoo]: https://sqlzoo.net/
[sql-nosql]: https://medium.com/xplenty-blog/the-sql-vs-nosql-difference-mysql-vs-mongodb-32c9980e67b2
[sql-w3]: https://www.w3schools.com/sql/sql_intro.asp
[rdbms-what]: https://www.codecademy.com/articles/what-is-rdbms-sql

</details>

## Day 3: Node-Postgres (`pg`), Express `Router()`

- Pre-Work:
  - [node-postgres (Sections: "Welcome" and "Queries")][pg-docs]

[pg-docs]: https://node-postgres.com/

| Topic                                   | Lecture                   | Slides                       | Demo                       | Solution                | Review |
| --------------------------------------- | ------------------------- | ---------------------------- | -------------------------- | ----------------------- | ------ |
| Node-Postgres (`pg`) (Wizard News Pt 2) |   | [🖼️][node-postgres-slides]   |   |  | -      |
| RESTful Routing (Wizard News Pt 3)      |  | [🖼️][restful-express-slides] | |  | -      |
| Morning Review                          |          | [🎟][am-rev-2-3-ticket]       | -                          | -                       | -      |

[//]: # ' Paste in table above >> [📺][node-postgres-lec] '
[node-postgres-lec]: https://youtu.be/-vSl7dyKfN4
[node-postgres-slides]: https://github.com/FullstackAcademy/2206-FSA-RM-WEB-FT/blob/main/01-junior-phase/day-7-pg-routes/node-postgres.pdf
[//]: # ' Paste in table above >> [🧑‍💻][node-postgres-demo] '
[node-postgres-demo]: https://github.com/FullstackAcademy/2206-FSA-RM-WEB-FT/tree/main/01-junior-phase/day-7-pg-routes/pg-demo
[//]: # ' Paste in table above >> [👾][wizard-news-2-sol] '
[wizard-news-2-sol]: https://github.com/FullstackAcademy/Solution.Wizard-news/tree/Part2
[//]: # ' Paste in table above >> [📺][wizard-news-2-rev] '
[wizard-news-2-rev]: ###
[//]: # ' Paste in table above >> [📺][restful-express-lec] '
[restful-express-lec]: https://youtu.be/CFK8Gefmivk
[restful-express-slides]: https://github.com/FullstackAcademy/2206-FSA-RM-WEB-FT/blob/main/01-junior-phase/day-7-pg-routes/express-routes-and-rest.pdf
[//]: # ' Paste in table above >> [🧑‍💻][restful-express-demo] '
[restful-express-demo]: https://github.com/FullstackAcademy/2206-FSA-RM-WEB-FT/tree/main/01-junior-phase/day-7-pg-routes/express-routes-REST
[//]: # ' Paste in table above >> [👾][wizard-news-3-sol] '
[wizard-news-3-sol]: https://github.com/FullstackAcademy/Solution.Wizard-news/tree/Part3
[//]: # ' Paste in table above >> [📺][wizard-news-3-rev] '
[wizard-news-3-rev]: ###
[//]: # ' Paste in table above >> [📺][am-rev-2-3] '
[am-rev-2-3]: https://youtu.be/WtAAyyjae68
[//]: # ' Paste in table above >> [🎟][am-rev-2-3-ticket] '
[am-rev-2-3-ticket]: https://forms.gle/SdRcKefq4qfYA1376
[//]: # ' Paste in table above >> [🧑‍💻][am-rev-2-3-demo] '
[am-rev-2-3-demo]: #link-demo-here
[//]: # ' Paste in table above >> [👾][am-rev-2-3-sol] '
[am-rev-2-3-sol]: #paste-gist-here

- **You should be able to:**
  - Describe the role of `pg` in our stack
  - Define REST and its advantages
  - Create and mount Express Routers
  - Explain the role of body parsing middleware

**<details><summary>📎 Extra Resources:</summary>**

- **PostgreSQL**
  - [Documentation][psql-docs]
  - [Tutorial][psql-tutorial]
- **[node-postgres (`pg`)](https://node-postgres.com/)**
  - [Features: Connecting](https://node-postgres.com/features/connecting)
  - [Features: Queries](https://node-postgres.com/features/queries)
  - [API: `pg.Client`](https://node-postgres.com/api/client)
- **Express & RESTful Routing**
  - [Gist: REST Anti-Patterns and Mistakes][rest-mistakes]
  - [RESTful API Resource Naming Convention][restful-api-naming]
  - Express has reincorporated body parsing starting with **v4.16**:
    - [Stackoverflow: `express.json` vs `bodyParser.json`][bparser-v-express]
  - [How bodyParser() works](https://medium.com/@adamzerner/how-bodyparser-works-247897a93b90)

[psql-docs]: https://www.postgresql.org/docs/8.0/tutorial.html
[psql-tutorial]: http://www.postgresqltutorial.com/
[rest-mistakes]: https://gist.github.com/omriBernstein/9f9c5f39afacc84faf44503fd64369cb
[restful-api-naming]: https://restfulapi.net/resource-naming/
[bparser-v-express]: https://stackoverflow.com/a/47232318

</details>

## Day 4: ORM (Sequelize), WikiStack 1

- Pre-Work:
  - [Sequelize An Introduction][sequelize-intro]

[sequelize-intro]: https://youtu.be/qsDvJrGMSUY

| Topic                     | Lecture                       | Slides           | Demo           | Solution              | Review                |
| ------------------------- | ----------------------------- | ---------------- | -------------- | --------------------- | --------------------- |
| Intro to ORMs (Sequelize) |  | [🖼️][orm-slides] |  |        | -                     |
| Wikistack 1               | -                             | -                | -              | | |
| Morning Review            |            | -                | -              | -                     | -                     |

[//]: # ' Paste in table above >> [📺][orm-lec] '
[orm-lec]: https://youtu.be/vcE47KwFOLc
[orm-slides]: https://docs.google.com/presentation/d/1MmXN7IE33tR2SytUO5Ko8tyVZFZ4qHwIb5ENCsrUYzQ/edit?usp=sharing
[//]: # ' Paste in table above >> [🧑‍💻][orm-demo] '
[orm-demo]: 01-junior-phase/day-8-orm-sequelize/sequelize-demo
[//]: # ' Paste in table above >> [📺][orm-lec-2] '
[orm-lec-2]: https://youtu.be/gX6ZmMyoMrg
[//]: # ' Paste in table above >> [👾][orm-sol] '
[orm-sol]: https://github.com/FullstackAcademy/Lab.Sequelize-First-Contact/tree/solution
[//]: # ' Paste in table above >> [👾][wikistack-1-sol] '
[wikistack-1-sol]: https://github.com/FullstackAcademy/Solution.Wikistack1
[//]: # ' Paste in table above >> [📺][wikistack-1-rev] '
[wikistack-1-rev]: https://www.youtube.com/playlist?list=PLx0iOsdUOUmmjZtJBNy8q-rajIBINW9t8
[//]: # ' Paste in table above >> [📺][am-rev-2-4] '
[am-rev-2-4]: https://youtu.be/0bfws2xt1JQ
[//]: # ' Paste in table above >> [🎟][am-rev-2-4-ticket] '
[am-rev-2-4-ticket]: #paste-google-form-link-here
[//]: # ' Paste in table above >> [🧑‍💻][am-rev-2-4-demo] '
[am-rev-2-4-demo]: #link-demo-here
[//]: # ' Paste in table above >> [👾][am-rev-2-4-sol] '
[am-rev-2-4-sol]: #paste-gist-here

- **You should be able to:**
  - Define an ORM, and explain its pros/cons
  - Define models in Sequelize
  - Associate models with each other
  - Hook into Sequelize lifecycle events
  - Query on models (`findAll`, `findOne`, `create`, "magic methods", etc)

**<details><summary>📎 Extra Resources:</summary>**

- [Official Sequelize Documentation](https://sequelize.org/master/)
- [How to Locate Magic Methods](https://gist.github.com/jbracht/1778e93ced532b902fc49d70a743ffb8)
- [Magic Methods Script](https://gist.github.com/b17z/916171a778c4ed7053d2052b0c6f7d55)
- [Lifecycle Methods](https://gist.github.com/Julissa93/6a6d29874d34a801d603d2522645025f)

</details>

## Day 5: WikiStack 2

- Pre-Work:
  - [Sequelize: Eager Loading][sequelize-eager]
  - [Sequelize: Instance & Class Methods][sequelize-methods]
  - [Express: Error Handling][express-error]

[sequelize-eager]: https://sequelize-guides.netlify.com/eager-loading/
[sequelize-methods]: https://sequelize-guides.netlify.com/instance-and-class-methods/
[express-error]: https://expressjs.com/en/guide/error-handling.html

| Topic                            | Lecture                | Slides                    | Demo                        | Solution              | Review |
| -------------------------------- | ---------------------- | ------------------------- | --------------------------- | --------------------- | ------ |
| Rounding Out Express & Sequelize |  | [🖼️][rounding-out-slides] |  | -                     | -      |
| Wikistack 2                      | -                      | -                         | -                           |  | -      |
| Morning Review                   |      | [🎟][am-rev-2-5-ticket]    | -                           | -                     | -      |

[//]: # ' Paste in table above >> [📺][rounding-out-lec] '
[rounding-out-lec]: https://youtu.be/40-AVLVUZIo
[rounding-out-slides]: https://docs.google.com/presentation/d/1QrlyvcJmexEATyZRBDr3D5GaU5rAqN_v4h9EK8xwYF0/edit?usp=sharing
[//]: # ' Paste in table above >> [🧑‍💻][rounding-out-lec-demo] '
[rounding-out-lec-demo]: https://github.com/FullstackAcademy/2206-FSA-RM-WEB-FT/tree/main/01-junior-phase/day-9-express-sequlize
[//]: # ' Paste in table above >> [👾][wikistack-2-sol] '
[wikistack-2-sol]: https://github.com/FullstackAcademy/Solution.Wikistack2
[//]: # ' Paste in table above >> [📺][am-rev-2-5] '
[am-rev-2-5]: https://youtu.be/AMZxiAtq8KY
[//]: # ' Paste in table above >> [🎟][am-rev-2-5-ticket] '
[am-rev-2-5-ticket]: https://forms.gle/x9FVcEtbuDyrxGBcA
[//]: # ' Paste in table above >> [🧑‍💻][am-rev-2-5-demo] '
[am-rev-2-5-demo]: #link-demo-here
[//]: # ' Paste in table above >> [👾][am-rev-2-5-sol] '
[am-rev-2-5-sol]: #paste-gist-here

- **You should be able to:**
  - Write custom error handlers in Express
  - Utilize eager loading in Sequelize queries
  - Write class and instance methods on Sequelize models

[Continue to 📆 Week 3](WEEK3.md)