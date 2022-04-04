# Class

* [Index](./Index.md)

## Example class code

```txt
public sealed namespace MyClass { 

    public struct MyStruct (
        internal my_value : Int
    );

    public funct New() : MyStruct {
        return MyStruct(0);
    }

    public sticky funct GetValue(this : MyStruct) : Int {
        return this.my_value;
    }

}

funct Main(args : String[]) : Int {

    data my_obj : MyClass.MyStruct = MyClass.New();
    data value : Int = my_obj.GetValue();

}
```
