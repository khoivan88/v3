# Instructions

In this exercise you'll be processing log-lines.

Each log line is a string formatted as follows: `"[<LEVEL>]: <MESSAGE>"`.

There are three different log levels:

- `INFO`
- `WARNING`
- `ERROR`

You have three tasks, each of which will take a log line and ask you to do something with it.

### 1. Get message from a log line

Implement a method to return a log line's message:

```go
Message("[ERROR]: Invalid operation")
// Returns: "Invalid operation"
```

Any leading or trailing white space should be removed:

```go
Message("[WARNING]:  Disk almost full\r\n")
// Returns: "Disk almost full"
```

### 2. Get the message length in characters

Implement a method to return a log line's message length:

```go
Strings.LogLevel("[ERROR]: Invalid operation \n")
// Returns: 17
```

### 3. Get log level from a log line

Implement a method to return a log line's log level, which should be returned in lowercase:

```go
Strings.LogLevel("[ERROR]: Invalid operation")
// Returns: "error"
```

### 4. Reformat a log line

Implement a method that reformats the log line, putting the message first and the log level after it in parentheses:

```go
Strings.Reformat("[INFO]: Operation completed")
// Returns: "Operation completed (info)"
```
