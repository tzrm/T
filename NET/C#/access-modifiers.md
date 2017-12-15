Access modifiers
----------------

* `public`
  
  The type or member can be accessed by any other code in the same assembly or another assembly that references it.
  
* `private`

  The type or member can only be accessed by code in the same class or struct.
  
* `protected`

  The type or member can only be accessed by code in the same class or struct, or in a derived class.
  
* `internal`

  The type or member can be accessed by any code in the same assembly, but not from another assembly.
  
* `protected internal`

  The type or member can be accessed by any code in the same assembly, or by any derived class in another assembly.
  
When no ***access modifier*** is set, a default access modifier is used. So there is always some form of access modifier even if it's not set.

* `static`

  The static modifier on a class means that the class cannot be instantiated, and that all of its members are static. A static member has one version regardless of how many instances of its enclosing type are created.

  A static class is basically the same as a non-static class, but there is one difference: a static class cannot be externally instantiated. In other words, you cannot use the new keyword to create a variable of the class type. Because there is no instance variable, you access the members of a static class by using the class name itself.

  However, there is a such thing as a static constructor. Any class can have one of these, including static classes. They cannot be called directly & cannot have parameters (other than any type parameters on the class itself). A static constructor is called automatically to initialize the class before the first instance is created or any static members are referenced. Looks like this:
  
``` C#
static class Foo()
{
    static Foo()
    {
        Bar = "fubar";
    }

    public static string Bar { get; set; }
}
```
