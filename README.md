# Dart: Handling `jsonDecode` FormatExceptions

This repository demonstrates a common error in Dart when using `jsonDecode` to parse JSON responses from APIs.  The original code lacks specific handling for `FormatException`, which can occur when the JSON is malformed or invalid. The solution provides robust error handling to address this issue, improving the application's resilience.

## Bug
The `bug.dart` file showcases the issue. It fetches data from an API and uses `jsonDecode`. If the API returns invalid JSON, the code throws a `FormatException`, which is not caught specifically, leading to application crashes or unexpected behavior.

## Solution
The `bugSolution.dart` file presents an improved version. It explicitly catches `FormatException` and handles it gracefully, providing more informative error messages and preventing application crashes.