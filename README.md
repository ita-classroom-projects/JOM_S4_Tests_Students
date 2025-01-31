# JOM. Generics. Collections. Annotations
## Task 7

Create a marker annotation **CamelCase** to check whether a method is named according to the code conventions. Create a class **CheckCamelCase** to verify if all the annotated methods of a given class satisfy the naming pattern. This class contains constant 'CAMELCASE_PATTERN' that defines a regex for checking method names. It also includes the method **checkAndPrint(Class clazz)** which returns true if all annotated methods in the given class conform to 'CAMELCASE_PATTERN'. Additionally, it prints to the standard output information about any incorrectly named methods using the following format: **method <className>.<methodName> doesn't satisfy camelCase naming convention**.

For example, for class
```java
public class Class1{
    @CamelCase
    public void correct(){}
    @CamelCase
    public void InCorrect(){}
    public void JustMethod(){}
}
```
call CheckCamelCase.checkAndPrint(Class1.class)

prints to console
```
method Class1.InCorrect doesn't satisfy camelCase naming convention
```

> For correct passing of all tests don't use any extra **print** and **println** methods in your code.
