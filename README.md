# PHP: Handling fopen() Failures Gracefully
This example demonstrates a common, yet subtle error in PHP file handling. The code attempts to close a file handle even if the `fopen()` operation failed.  While PHP doesn't throw an error, it's bad practice.  The improved version adds a check to ensure `fopen()` was successful before closing the file handle.

This repository contains two files:
- `bug.php`: Shows the problematic code.
- `bugSolution.php`: Provides the corrected code.