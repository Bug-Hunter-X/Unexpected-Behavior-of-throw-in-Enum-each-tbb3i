# Elixir Enum.each and throw Unexpected Behavior

This repository demonstrates an unexpected behavior when using `throw` within an `Enum.each` loop in Elixir.  The `throw` statement doesn't behave intuitively in this context.  See `bug.ex` for the problematic code and `bugSolution.ex` for a corrected approach.

The core issue lies in the fact that `throw` terminates execution of the entire function, not just the current iteration of the loop.  This behavior is different from exceptions in some other languages.

This example highlights the importance of understanding the specifics of Elixir's exception handling and the proper use of `Enum.each`, `Enum.map`, and alternatives for handling exceptional conditions within loops.