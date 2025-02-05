# Separate read and write

## Usecase

- Data provider is external service.
- There are many requests at Frontend.

## components

```
Frontend
|
DataReader
|
Database
|
DataWriter (pull, push, etc..)
|
--- Boundary of internal and external ---
|
DataProviderService
```
