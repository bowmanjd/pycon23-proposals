# Upside-down SQLAlchemy: Moving Structure and Data between Different Database Engines 

Track: Talks
Category: Data Processing

## Description

SQLAlchemy allows a Python developer to write generic database manipulation code that works with a variety of database engines. Yet SQLAlchemy can also go the opposite direction, generating SQL and extracting data from an already established database, using reflection and generic types. Consider moving data and schema from PostgreSQL to Microsoft SQL Server, or from SQLite to PostgreSQL. This talk explores methods and possibilities for such migration. 

## Outline

Introduction (1 minute)

The challenge of data and schema between database engines (5 minutes)
- So similar, yet... (highlighting some differences in SQL syntax and types)
- Scenarios in which automated abstraction is desirable

SQLAlchemy summary (5 minutes)
- Core vs ORM
- SQL expression language (pythonic SQL!)
- DDL: tables, models, types (from Python to SQL and back again)
- Some supported database engines: SQLite, PostgreSQL, MySQL/MariaDB, Oracle, Microsoft SQL

Discovering and defining schema (5 minutes)
- reflect
- generic types

Extracting and inserting data (5 minutes)
- SQLAlchemy all the way
- Speedy alternative: aim for the bulk loader (such as Microsoft's bcp or PostgreSQL's COPY)

Additional tooling (1 minute)
- sqlacodegen

Discussion (5 minutes)

## Past experience

Currently a software engineer using SQL to convert data between systems, I have been a middle and high school teacher, software developer, IT director, data wrangler, and always a hobbyist developer. I feel comfortable in front of people.
