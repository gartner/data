# Agile Data - Domain Model and Persistence library


Most performance problems in apps are tend to arise due to inefficient use of database access patterns. In practical applications, when you have a strict deadline, developers are forced to make trade-offs that result in poor scalability or poor application design.

 1. It's hard to implement Domain Model and Persistance separation within reasonable time.
 2. Query Building, ORM and ActiveRecord lack synergy in most frameworks.
 3. Each pattern to access database falls short making you fall back to SQL.

Agile Data is a unique library that enforces correct design of Business Logic in your PHP
application and handles persistence (interaction with database) in flexible and scalable way.

 - **Full separation** between your Domain Model and Persistence in a **practical way**.
 - Query Builder, Relations and Active Record that work in **great synergy**.
 - Any Query policy. You will **no longer** have excuse to **write raw queries**.
 - Use power of **SQL** with PDO-databases, while also being compatible with **NoSQL** databases.

## Concept Explained

To learn Agile Data, you need to leave behind your prejudice towards some of the data access
patterns and read on how we are turning familiar concepts by implementing them correctly:

 - [Business Models](https://github.com/atk4/dataset/wiki/Business-Models) - Class for implementing your business logic [DM].
 - [Active Record](https://github.com/atk4/dataset/wiki/Active-Record) - Simplified record-based access to your Model data. [DM].
 - [Explicit Loading and Saving](https://github.com/atk4/dataset/wiki/Explicit-Loading-and-Saving) - No auto-load/auto-save. Learn how to access your database data [PM].
 - [Relation Mapping](https://github.com/atk4/dataset/wiki/Relation-Mapping) - Traverse between related business data [DM].
 - [Persistence](https://github.com/atk4/dataset/wiki/Persistence) - Design and tweak how your Business Models are mapped into tables [DM->PM].
 - [Derived Queries](https://github.com/atk4/dataset/wiki/Derived-Queries) - Express your Business Models as SQL queries [PM].
 - [Expressions](https://github.com/atk4/dataset/wiki/Expressions) - Use Derived queries to add fields in your Business Models that are calculated in SQL [PM].
 - [Query Building](https://github.com/atk4/dataset/wiki/Query-Building) - Build an execute complex multi-row queries mapped from your Business Models [PM].
 - [Unit-testing](https://github.com/atk4/dataset/wiki/Unit-Testing) - Business Models can be decoupled from persistence layer for efficient Unit Testing [DM].
 - [Aggregation and Reports](https://github.com/atk4/dataset/wiki/Aggregaation-and-Reports) - Support report generation techniques, aggregation and unions for your Business models [DM].

All of the above concepts are designed and delivered in a very simple-to-learn way. Our main goal is to educate new programmers about the right way to write code through intuitive pattern designs.

We also care about other technicalities, so we will:

 - work with PHP community and discuss main decisions collaboratively. 
 - write short and easy-to-read, standard-compliant code with high code-climate score.
 - unit-test our own code with minimum of 95% code coverage.
 - never break APIs in minor releases.
 - include minimum dependencies.
 - be friendly with all higher-level frameworks.
 - avoid database query latency/overheads, pre-fetching or lazy loading.
 - do not duplicate the code (e.g. in vendor drivers)
 - use MIT License

The founder and lead developer for this library is: [Romans Malinovskis](https://www.openhub.net/accounts/romaninsh). To get in touch privately, [use my twitter](https://twitter.com/romaninsh).

[Frequently Asked Questions](https://github.com/atk4/dataset/wiki/Frequently-Asked-Questions)

## Current Status

We are currently working on "Concept Design". Feel free to discuss, contribute feedback or follow. 

[Read our Development Wiki](https://github.com/atk4/dataset/wiki).

You can also join us on Gitter to ask questions:

[![Join the chat at https://gitter.im/atk4/dataset](https://badges.gitter.im/atk4/dataset.svg)](https://gitter.im/atk4/dataset?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

## Roadmap

To implement Agile Data, we had to start from the very beginning.

```
0.1   Finalize concept, api-interface draft and lightweight documentation, before any code is written.
0.2   Implement Active Record with Business Model class.
0.3   Implement SQL persistence mapping - storing and loading records.
0.4   Add support for Conditions to implement DataSet.
0.5   Further integrate with the Query Builder, add Expression support.
0.6   Add relation traversal support.
0.7   Add support for hooks (before/after save) in (DM and PM).
0.8   Add support for dealing with multiple persistences.
0.9   Add support for strong and weak join when persisting.
0.10  Add ability to specify meta-information into fields.
0.11  Add support for derived models (unions).
1.12  Add support for 3rd party vendor implementations.
0.13  Achieve our test coverage, code quality and documentation standards.
1.0   First Stable Release.
1.1   Add support for MongoDB.
1.2   Add support and docs for Validators.

## Past Updates

* 17 Apr: Started working on draft concept (in wiki)
* 14 Apr: [Posted my concept on Reddit](https://www.reddit.com/r/PHP/comments/4f2epw/reinventing_the_faulty_orm_concept_subqueries/)



