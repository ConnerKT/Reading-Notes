# LINQ & Delegates

This topic is important to me because I want to be able to perform SQL like queries directly on collections like arrays, lists, and DB's.

## [Retrospective 9](https://connerkt.github.io/Reading-Notes/401/Class09/Retro09)

## References

[LINQ](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/)

[Intro to LINQ Queries](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/introduction-to-linq-queries)

[Basic LINQ Query Operations](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/basic-linq-query-operations)

[Walkthrough Writing LINQ Queries](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/walkthrough-writing-queries-linq)

## LINQ

- **Overview**
  - **Language Integrated Query (LINQ):** Simplifies querying data from different sources using a unified syntax.
  - **Expressive Queries:** Enables SQL-like queries for improved code readability.
  - **Data Sources:** Works with arrays, databases, XML, and more.

- **Benefits**
  - **Enhanced Productivity:** Reduces code and boosts developer efficiency.
  - **Readability:** Concise queries resemble natural language, aiding maintainability.
  - **Type Safety:** Strong typing reduces runtime errors.

- **Components**
  - **LINQ to Objects:** Manipulates in-memory data (e.g., arrays).
  - **LINQ to SQL:** Queries relational databases.
  - **LINQ to XML:** Manipulates XML data.
  - **LINQ to Entities:** Works with Entity Framework for data querying.

- **Query Structure**
  - **Keywords:** Utilizes `from`, `where`, `select`, and more.
  - **Fluent Syntax:** Supports method chaining.
  - **Deferred Execution:** Lazily evaluates queries.

- **Query Operators**
  - **Standard Operators:** Includes `Where`, `Select`, `OrderBy`, and more.
  - **Custom Operators:** Extend LINQ's functionality.

- **Examples**
  - **Filtering:** `Where` to filter based on conditions.
  - **Projection:** `Select` for extracting specific data.
  - **Sorting:** `OrderBy` for data sorting.
  - **Grouping:** `GroupBy` to group based on attributes.
  - **Joining:** `Join` to combine data from sources.

- **Performance**
  - **Optimization:** Understand execution and optimization for better performance.
  - **Materialization:** Awareness of data retrieval impacts performance.

- **Integration**
  - **Anonymous Types:** Often used to structure query results.
  - **Implicit Typing:** `var` for type inference with LINQ.

## Introduction to LINQ Queries

All LINQ query operations consist of three distinct actions:

1. Obtain the data source.

2. Create the query.

3. Execute the query.

## LINQ Query Operations

LINQ (Language Integrated Query) is a feature in C# that enables data querying and manipulation within your code. LINQ supports query syntax and method syntax for defining queries.

### 1. Filtering

- `Where`: Filters elements based on a specified condition.
- `OfType`: Filters elements to include only those of a specified type.

### 2. Projection

- `Select`: Projects each element of a collection into a new form.
- `SelectMany`: Projects and flattens a collection of collections.

### 3. Ordering

- `OrderBy`: Orders elements in ascending order based on a specified key.
- `OrderByDescending`: Orders elements in descending order based on a specified key.

### 4. Grouping

- `GroupBy`: Groups elements by a specified key and creates groups of elements with the same key.

### 5. Aggregation

- `Count`: Counts the number of elements in a collection.
- `Sum`: Computes the sum of values in a collection.
- `Average`: Computes the average of values in a collection.

### 6. Joining

- `Join`: Joins two collections based on a common key.
- `GroupJoin`: Joins two collections and groups the results based on a common key.

### 7. Set Operations

- `Union`: Combines two collections, removing duplicates.
- `Intersect`: Finds elements common to both collections.
- `Except`: Finds elements in one collection not in another.

LINQ Query Operations provide a concise and readable way to perform complex data manipulations.

## Things I want to know more about

I want to know more about when LINQ is used in bigger companies and how useful it is.

I want to learn more about using LINQ queries on my API call data.