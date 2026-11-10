# PenguEats Inventory Management System

A command-line inventory management system (C++) for PenguEats, a fictional seafood restaurant for penguies.
This repository and project are being created and developed for the course "Project: General Programming with C/C++" at IU: International University of Applied Sciences.

## Architecture
(Initial prediction. Possible changes in the future)

### Projected operations:
- Add, edit, deactivate, list, search, and sort ingredients;
- Record transactions to provide a traceable history of stock movements and changes;
- Generate exportable reports containing useful insights;

### Entities of the project:

- Supplier: id [int], name [string], contact [string]
- Ingredient: id [int], name [string], description [string], category [enum], freshness [enum], expiresAt [TimePoint], cost [double], quantity [int], minStock [int], supplierId [int], createdAt [TimePoint]
- Transaction: id [int], ingredientId [int], type [enum], supplierId [int], amount [int], note [string], timestamp [TimePoint]
- LogEntry: id [int], timestamp [TimePoint], entityType [enum], entityId [int], details [string], action [enum] 

### File format and persistence
Data will be saved in a single CSV file with semicolons as field separators, as well as properties (e.g., headers) useful for maintenance and traceability.

### Toolchain
- C++ version 20
- G++
- CMake
- Git (and GitHub)
- Catch2

### Author:
Bruno Santos