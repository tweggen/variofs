localvariofs

This is a worker service that executes a given configuration for the 
variofs file application.

In usual modes of operation, it observes a couple of folders or drives
on your hard drive for changes, making them available upstream for other
parts of your backup strategy.


Prototype implementation:

local driver:
- read json configuration
  - list of directories to go upstream

- update local internal caching database from filesystem (note: DB is 
  just an internal optimization)

