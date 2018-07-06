#What is String Interning ?

String Interning is a method of storing only one copy of each distinct String Value, which must be immutable.

In Java, String class has a public method intern() that returns a canonical representation for the string object. Java’s String class privately maintains a pool of strings, where String literals are automatically interned.

The intern() method helps in comparing two String objects with == operator by looking into the pre-existing pool of string literals, no doubt it is faster than equals() method. The pool of strings in Java is maintained for saving space and for faster comparisons.Normally Java programmers are advised to use equals(), not ==, to compare two strings. This is because 

### == operator compares memory locations
### equals() method compares the content stored in two objects.

#Why and When to Intern ?

Though Java automatically interns all Strings by default, remember that we only need to intern strings when they are not constants, and we want to be able to quickly compare them to other interned strings. The intern() method should be used on strings constructed with new String() in order to compare them by == operator.
