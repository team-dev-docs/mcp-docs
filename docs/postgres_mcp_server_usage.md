

  # Using the Postgres MCP Server

This guide covers how to use the Postgres Model Context Protocol (MCP) server to connect to a Postgres database, execute queries, and manage database resources.

## Getting Started

The Postgres MCP server allows you to interact with a Postgres database using the Model Context Protocol. To use it, you'll need:

1. The Postgres MCP server code
2. A Postgres database URL

## Connecting to a Database

To start the server and connect to your database:

1. Run the server with your database URL as an argument:

```bash
node src/postgres/index.js postgresql://username:password@host:port/database
```

The server will establish a connection pool to your database using the provided URL.

## Listing Database Resources

The server exposes database tables as resources. To list available resources:

1. Send a `ListResourcesRequest` to the server
2. The server will query the database for table names in the public schema
3. It returns a list of resources, with each table represented as a resource URI

Example response:

```json
{
  "resources": [
    {
      "uri": "postgres://host:port/database/users/schema",
      "mimeType": "application/json",
      "name": "\"users\" database schema"
    },
    {
      "uri": "postgres://host:port/database/products/schema",
      "mimeType": "application/json",
      "name": "\"products\" database schema"
    }
  ]
}
```

## Reading Resource Information

To get information about a specific table:

1. Send a `ReadResourceRequest` with the resource URI
2. The server queries the database for column information
3. It returns the table schema as JSON

Example request:

```json
{
  "params": {
    "uri": "postgres://host:port/database/users/schema"
  }
}
```

Example response:

```json
{
  "contents": [
    {
      "uri": "postgres://host:port/database/users/schema",
      "mimeType": "application/json",
      "text": [
        {
          "column_name": "id",
          "data_type": "integer"
        },
        {
          "column_name": "username",
          "data_type": "character varying"
        },
        {
          "column_name": "email",
          "data_type": "character varying"
        }
      ]
    }
  ]
}
```

## Executing Queries

To run SQL queries:

1. Send a `CallToolRequest` with the "query" tool
2. Provide your SQL query in the `arguments.sql` field
3. The server executes the query in a read-only transaction
4. It returns the query results as JSON

Example request:

```json
{
  "params": {
    "name": "query",
    "arguments": {
      "sql": "SELECT * FROM users LIMIT 5"
    }
  }
}
```

Example response:

```json
{
  "content": [
    {
      "type": "text",
      "text": [
        {
          "id": 1,
          "username": "john_doe",
          "email": "john@example.com"
        },
        {
          "id": 2,
          "username": "jane_smith",
          "email": "jane@example.com"
        }
      ]
    }
  ],
  "isError": false
}
```

## Error Handling

- If an invalid resource URI is provided, the server will throw an error.
- SQL query errors will be caught and returned as exceptions.
- Failed transactions are automatically rolled back.

## Limitations

- The server currently only supports read-only operations.
- Only tables in the public schema are accessible.
- The server does not support authentication or authorization beyond the initial database connection.

By following this guide, you can effectively use the Postgres MCP server to interact with your Postgres database through the Model Context Protocol.

  