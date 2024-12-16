# Elixir Enum.reduce and Empty List Handling

This repository demonstrates a potential issue with `Enum.reduce` in Elixir when dealing with empty or nil lists and provides a solution.

The `bug.ex` file contains Elixir code that uses `Enum.reduce` to sum elements greater than 3.  However, it lacks robust error handling for empty lists.

The `bugSolution.ex` file provides a corrected version with improved error handling.

## Bug
The original code fails gracefully when encountering an empty list, returning 0 which is not always the desired behavior.  A nil list will cause a crash.

## Solution
The solution introduces a check for an empty list before using `Enum.reduce`. This prevents unexpected behavior or crashes.