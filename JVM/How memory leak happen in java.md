# What is a leak?

>The standard definition of a memory leak is a scenario that occurs when objects are no longer being used by the application, but the Garbage Collector is unable to remove them from working memory – because they’re still being referenced. As a result, the application consumes more and more resources – which eventually leads to a fatal OutOfMemoryError.

# How does leak happen
## 1. Static Field Holding onto the Object reference
## 2. Calling String.intern() on Long String
