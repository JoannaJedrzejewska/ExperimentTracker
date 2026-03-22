# ExperimentTracker
A lightweight experiment tracking system built with Python and SQLAlchemy ORM.  
Stores experiments and their associated data points in a local SQLite database,  
with full CRUD support and relationship management.

## Features

- **ORM Models** – `Experiment` and `DataPoint` with a one-to-many relationship
- **Full CRUD** – insert, query, update, and delete via SQLAlchemy Core & ORM
- **Cascade delete** – removing an experiment automatically removes its data points
- **Schema inspection** – runtime table/column/foreign key introspection via `Inspector`
- **DB reset** – `drop_database()` clears the SQLite file for a clean slate
- **Session management** – context-managed sessions (`with SessionLocal()`)
