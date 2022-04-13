# Rose Programming Language

* [Index](Index.md)

## Basic topics

* [Datas](#datas)
* [Structures](#structures)
* [Functions](#functions)

## Datas

A *Data* is a named memory storage space. A *Data* has a type that defines the memory storage layout and size. Use the next syntax to define a *Data*:

```data DID: TYPE;```

> * DID refers to "Data IDentifier"
> * TYPE refers to any type

This syntax reserves the required memory for the type *TYPE* and then tagged it with the name *DID*. This syntax **DO NOT INITIALIZE** the content of the data only reserves its size.

To update the content of the data use the next syntax:

```DID = EXP;```

> * EXP refers to any aritmethic/logic/calling/coding expression

This syntax replaces the content of the *Data* with the result of an *Expression*. The *Expression* result type must match with the *Data* type.

See also:

* [Operators](Code/Operators.md)

## Structures

A *Structure* is a way to group data using a specific layout. A *Strcuture* has a name that defines its own *Type* and a list of data members with their own names and types. The next syntax defines a *Structure*:

```struct SID(MID: Type, ... );```

> * SID refers to "Structure IDentifier"
> * MID refers to "Member IDentifier"

This syntax defines the memory layout of the *Structure* type and then tag it with the name *SID*.

To use the *Struct* use it like other *Type*:

```data DID: SID;```

And then access to its members using:

```DID.MID = EXP;```

See also:

* [Constructors](Data/Constuctors.md)

## Functions

A *Function* is a block of code that can be executed by a call to it. A *Function* has list of parameters with their own names and types, and a return *Type*. The next syntax defines a *Functions*:

```funct FID(PID: TYPE, ...) TYPE { ... }```

> * FID refers to "Function IDentifier"
> * PID refers to "Parameter IDentifier"

To use a *Function* by calling it with the next syntax:

```FID(EXP, ...);```

See also:

* [Code Blocks](Code/Blocks.md)
