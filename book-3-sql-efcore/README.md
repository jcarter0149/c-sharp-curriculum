# Book 3 - Managing Data with SQL and Entity Framework Core
Up until now in the server-side course, we have been using variables in our programs to store the data for our applications (storing the data _in-memory_). Of course, this doesn't work in real-life situations. It's rare that applications like those that we're building don't require permanent data storage. When you shut down the apps that you've built thus far, any changes to them are discarded along with any other data the application stored in your computer's memory while it was running. 

In the front-end course, you used a JSON data file to store data (and data changes!) that will persist between runs of the application. In this book you will learn to use a number of technologies to do this instead:
1. **PostgreSQL** - a relational database that will store data in a number of files in a directory on your computer.  PostgreSQL is an application that can read and write data to those files, and is listening for network requests to do those operations. 
1. **SQL** - (Structured Query Language) a language used by many relational databases to provide the ability to _query_ the data stored in the database, as well as make changes to that data. Every relational database implements SQL slightly differently, though the skills learned in using one system largely transfer to the others, especially at the conceptual level (but largely the syntax as well). Some other relational databases are called Oracle, SQL Server, and MySQL.
1. **Entity Framework Core** - EF Core is set of .NET packages that allow your .NET application to send _SQL queries_ to the _PostgreSQL_ server. _Postgres_ will execute that query, and return the data, if any, that the query produced. EF Core will receive that response, and turn the data into C# objects that you can use in your application.

Because of the large scope of this book, it is split into three parts, roughly corresponding to the three technologies above. Start with the installations, and work your way down. Complete every column in a specific part before moving on to the next part:

|[Installations for Book 3](./chapters/book-3-installs.md) :computer: |
|--|

## I. Learning to write SQL

|:zap: [Getting started with SQL Bolt](https://sqlbolt.com/)|
|-|
|:elephant: [Creating a PostgreSQL database using pgAdmin](./chapters/music-history-setup.md)|
|:headphones: [Music History](./chapters/music-history-practice.md) |
|:page_with_curl: [Using SQL scripts to create databases](./chapters/poki-setup.md)|
|:black_nib: [Poems By Kids](./chapters/poki-practice.md)|

## II. Querying a SQL database from a Web API
| # |🍯💻 Honey Rae's API|
|-|-|
|1| [Creating a database for Honey Rae's API](./chapters/honey-rae-database.md) |
|2| [Using Npgsql to make our first query](./chapters/honey-res-npgsql.md) |
|3| [Getting related data](./chapters/honey-raes-related-data.md) |
|4| [Inserting and Updating rows](./chapters/honey-raes-create.md) |
|5| [Deleting a row](./chapters/honey-raes-delete.md) |
## III. Entity Framework Core
|#|:tent: <br> Creek River Campground <br> (guided tour) | :book: <br> Loncotes County Library | :haircut: <br> Hillary's Hair Care |
|:-:|:-:|:-:|:-:|
|1| Project Setup |||
|2| Adding Models |||
|3| Creating the database |||
|4| Get reservations and sites |||
|5| Get reservation details |||
|6| Book reservations |||
|7| Delete a reservation |||
|8| Delete a campsite |||
|9| Update a campsite |||

## 🔍 Additional Materials
|:compass: Explorer Chapters|
|-|
|🍯 💻 Finishing Honey Rae's with Npgsql |
|🍯 💻 Following the SRP with the Repository Pattern |
|🍯 💻 Handling Related Data On Delete |