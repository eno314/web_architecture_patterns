# Separate read and write

## Usecase

- Data provider is external service.
- There are many requests at Frontend.
  - It can use cache at DataReader or between Frontend and DataReader.

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
