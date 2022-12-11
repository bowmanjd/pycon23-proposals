# Upside-down SQLAlchemy: Moving Structure and Data between Different Database Engines 

Track: Talks
Category: Data Processing

## Description

SQLAlchemy allows a Python developer to write generic database manipulation code that works with a variety of database engines. Yet SQLAlchemy can also go the opposite direction, generating SQL and extracting data from an already established database, using reflection and generic types. Consider moving data and schema from PostgreSQL to Microsoft SQL Server, or from SQLite to PostgreSQL. This talk explores methods and possibilities for such migration. 

## Outline

Introduction (1 minute)

The challenge of data and schema between database engines (5 minutes)
* So similar, yet... (highlighting some differences in SQL syntax and types)
* Scenarios in which automated abstraction is desirable

SQLAlchemy summary (5 minutes)
* Core vs ORM
* SQL expression language (pythonic SQL!)
* DDL: tables, models, types (from Python to SQL and back again)
* Some supported database engines: SQLite, PostgreSQL, MySQL/MariaDB, Oracle, Microsoft SQL

Discovering and defining schema (5 minutes)
* reflect
  * How to reflect an entire database
	* Greater selectivity by filtering tables
* generic types in SQLAlchemy
* Putting it together: passing a genericizing function to reflect
* Customizing per column type, where needed

Extracting and inserting data (5 minutes)
* SQLAlchemy all the way
  * Read from one connection/engine, write to another
	* Paging for performance
* Speedy alternative: aim for the bulk loader (such as Microsoft's bcp or PostgreSQL's COPY)
  * Export using SQLAlchemy, customizing the output file format as is relevant for the bulk tool
	* Pay attention to delimiters and escaping!
	* Load with the appropriate tool and watch the data fly by

Additional tooling (1 minute)
* sqlacodegen

Discussion (5 minutes)

## Past experience

Currently a software engineer using SQL to convert data between systems, I have been a middle and high school teacher, software developer, IT director, data wrangler, and always a hobbyist developer. I feel comfortable in front of people.

I just presented at OLF (Ohio LinuxFest) on December 2, 2022, on using Python to manage Linux systems. Slides are available at olf22.bowmanjd.com and the video can be viewed on Youtube at https://youtu.be/DjOgRbHnvwU?t=465 (should start around 7 minutes, 45 seconds in).

A slide deck for a 2019 talk I gave at a local tech conference, introducing Python to IT professionals: bowmanjd.github.io/ttl/python-data/#1

linkedin.com/in/jonathan-d-bowman/
twitter.com/jdbowman
Various blog articles at dev.to/bowmanjd
