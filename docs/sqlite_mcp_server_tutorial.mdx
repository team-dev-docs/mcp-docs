

  # Using the SQLite MCP Server

This tutorial will walk you through how to use the SQLite Model Context Protocol (MCP) server to create and manage databases, execute queries, and leverage the server for data analysis tasks.

## Overview

The SQLite MCP server provides an interface to interact with SQLite databases through the Model Context Protocol. It allows you to:

- Create and manage SQLite databases
- Execute SQL queries to read and write data  
- Define database schemas and tables
- Analyze data and generate insights

The server exposes several tools and resources that can be used by AI assistants or other clients to work with SQLite databases in an interactive way.

## Getting Started

To use the SQLite MCP server:

1. Ensure you have the server installed and running
2. Connect to the server using an MCP client 
3. Use the available tools and resources to interact with the database

## Key Concepts

The SQLite MCP server provides the following key components:

- **Tools** - Functions to execute database operations
- **Resources** - Accessible data like the insights memo
- **Prompts** - Pre-defined templates to guide interactions

## Available Tools

The server exposes the following tools:

- `read_query` - Execute SELECT queries to read data
- `write_query` - Execute INSERT, UPDATE, or DELETE queries to modify data
- `create_table` - Create new tables in the database  
- `list_tables` - Show all existing tables
- `describe_table` - Show the schema for a specific table
- `append_insight` - Add a new business insight to the memo resource

## Creating and Managing Databases

### Creating a New Table

To create a new table, use the `create_table` tool:

```python
create_table_result = await server.call_tool("create_table", {
  "query": """
    CREATE TABLE users (
      id INTEGER PRIMARY KEY,
      name TEXT NOT NULL,
      email TEXT UNIQUE NOT NULL
    )
  """
})
```

### Listing Tables

To see all tables in the database:

```python
tables = await server.call_tool("list_tables", {})
```

### Describing a Table

To view the schema of a specific table:

```python 
schema = await server.call_tool("describe_table", {
  "table_name": "users"
})
```

## Executing Queries

### Reading Data

To execute a SELECT query:

```python
results = await server.call_tool("read_query", {
  "query": "SELECT * FROM users WHERE id = 1"
})
```

### Writing Data

To insert, update or delete data:

```python
result = await server.call_tool("write_query", {
  "query": "INSERT INTO users (name, email) VALUES ('Alice', 'alice@example.com')"
})
```

## Data Analysis

### Generating Insights

As you analyze data, you can add insights to the memo resource:

```python
await server.call_tool("append_insight", {
  "insight": "User signups increased 25% after the new marketing campaign"
})
```

### Accessing the Insights Memo

The insights memo is available as a resource:

```python
memo = await server.read_resource("memo://insights")
```

This memo is automatically updated as new insights are added.

## Using Prompts

The server provides a demo prompt to showcase its capabilities:

```python
prompt = await server.get_prompt("mcp-demo", {"topic": "retail sales"})
```

This prompt guides you through creating a sample database, running queries, and generating insights for a given business scenario.

## Best Practices

- Use parametrized queries when possible to prevent SQL injection
- Leverage the insights memo to keep track of important findings
- Use the demo prompt as a starting point to learn the server's capabilities

## Conclusion

The SQLite MCP server provides a powerful interface for interacting with SQLite databases programmatically. By leveraging its tools and resources, you can easily create databases, execute queries, and perform data analysis tasks in an interactive and AI-assisted manner.

  