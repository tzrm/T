## How to use value type parameters

``` C#
class Program
    {
        static void Main(string[] args)
        {
            new A<string>("myString"); // error: The type 'string' must be a non-nullable value type in order to use it as
                                       //        parameter 'T' in the generic type or method 'A<T>'
            new A<int>(4);
            new A<double>(4.4);
        }
    }

    public class A<T> where T : struct
    {
        public A(T value)
        {
            Console.WriteLine(value);
        }
    }
```
