# Kotlin MutableSet removeIf ConcurrentModificationException

This repository demonstrates a subtle difference in behavior between `MutableList` and `MutableSet` when using the `removeIf` function in Kotlin.  Modifying a `MutableSet` while iterating using `removeIf` leads to a `ConcurrentModificationException`, whereas `MutableList` handles it gracefully.

The `bug.kt` file showcases the issue, while `bugSolution.kt` presents a solution using an iterator for safe removal.

This example highlights the importance of understanding the underlying data structures and iteration mechanisms when working with Kotlin collections.