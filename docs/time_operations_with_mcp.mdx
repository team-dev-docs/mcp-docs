

  # Using the Time MCP Server

The Time MCP server provides tools for performing time-related operations, including getting the current time in different timezones and converting times between timezones.

## Available Tools

The Time MCP server offers two main tools:

1. `get_current_time` - Get the current time in a specific timezone
2. `convert_time` - Convert a time from one timezone to another

## Getting the Current Time

To get the current time in a specific timezone, use the `get_current_time` tool.

### Input

The tool requires a single input:

- `timezone`: The IANA timezone name (e.g., 'America/New_York', 'Europe/London')

If no timezone is specified, the server will use the local timezone.

### Example Usage

```json
{
  "timezone": "America/New_York"
}
```

### Output

The tool returns a JSON object with the following fields:

- `timezone`: The timezone name
- `datetime`: The current date and time in ISO 8601 format
- `is_dst`: A boolean indicating whether daylight saving time is in effect

Example output:

```json
{
  "timezone": "America/New_York",
  "datetime": "2023-04-15T14:30:00-04:00",
  "is_dst": true
}
```

## Converting Time Between Timezones

To convert a time from one timezone to another, use the `convert_time` tool.

### Input

The tool requires three inputs:

- `source_timezone`: The source IANA timezone name
- `time`: The time to convert in 24-hour format (HH:MM)
- `target_timezone`: The target IANA timezone name

### Example Usage

```json
{
  "source_timezone": "America/New_York",
  "time": "14:30",
  "target_timezone": "Asia/Tokyo"
}
```

### Output

The tool returns a JSON object with the following fields:

- `source`: Object containing source timezone information
- `target`: Object containing target timezone information
- `time_difference`: String representing the time difference between timezones

Example output:

```json
{
  "source": {
    "timezone": "America/New_York",
    "datetime": "2023-04-15T14:30:00-04:00",
    "is_dst": true
  },
  "target": {
    "timezone": "Asia/Tokyo",
    "datetime": "2023-04-16T03:30:00+09:00",
    "is_dst": false
  },
  "time_difference": "+13h"
}
```

## Error Handling

The server will return an error message if:

- An invalid timezone is provided
- Required arguments are missing
- The time format is incorrect (should be HH:MM in 24-hour format)

Example error:

```json
{
  "error": "Invalid timezone: Unknown timezone"
}
```

## Notes

- The server uses IANA timezone names. Make sure to use the correct format (e.g., 'America/New_York' instead of 'EST' or 'Eastern Time').
- All times are returned in ISO 8601 format.
- The server automatically handles daylight saving time adjustments.

  