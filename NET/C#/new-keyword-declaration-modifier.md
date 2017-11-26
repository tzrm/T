`new` keyword as a declaration modifier
---------------------------------------

When used as a declaration modifier, the `new` keyword explicitly hides a member that is inherited from a base class. When you hide an inherited member, the derived version of the member replaces base class version, Although you can hide members without using the new modifier, you get a compiler warning. If you use `new` to explicitly hide a member, it suppresses this warning.
To hide an inherited member, declare it in the deriver class by using the same member name, and modify ti with the new keyword.
For example

```C#
public class BaseC
{
  public int x;
  public void Invoke() {}
}

public class DerivedC : BaseC
{
  new public void Invoke() {}
}
```
