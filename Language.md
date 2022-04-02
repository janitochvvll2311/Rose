# Sketch

## Declaration and definition syntaxes

### Structure entity

``` txt
struct <ID>;          // Declaration


struct <ID> (         // Definition
    <ID> : <TYPE>,    // Data member
    <ID> : <TYPE>,    // Data member
    ...
);
```

Structure details

``` txt
struct Sx;              // Declaration
struct Sx (M, M, ...);  // Definition
Sx(D, D, ...)           // Expresion
```

### Function

``` txt
funct <ID> (          // Declaration
    <ID> : <TYPE>,    // Data member
    <ID> : <TYPE>,    // Data member
    ...
) : <TYPE>;             // Return type          


funct <ID> (          // Definition
    <ID> : <TYPE>,    // Data member
    <ID> : <TYPE>,    // Data member
    ...
) : <TYPE> {            // Code block
    ...
};
```

Function details

``` txt
funct Fx (M, M, ...) : Tx;          // Declaration
funct Fx (M, M, ...) : Tx {...};    // Definition
Fx(D, D, ...)                       // Expresion
```

### Data

``` txt
data <ID> : <TYPE>;       // Declaration


data <ID> : <TYPE>        // Definition
    = <EXP>
```

Data details

``` txt
data Dx : Tx;           // Declaration
data Dx : Tx(D, ...);   // Definition
Dx : Tx(D, ...)         // Expresion
```

## Syntax comparison

| Name | Syntax
| - | -
| Structure declaration | ```struct <ID>;```
| Function declaration | ```funct <ID> ( <ID> : <TYPE>, ... ) : <TYPE>;```
| Data declaration | ```data <ID> : <TYPE>;```
| Structure definition | ```struct <ID> ( <ID> : <TYPE>, ... );```
| Function definition | ```funct <ID> ( <ID> : <TYPE>, ... ) : <TYPE> { ... };```
| Data definition | ```data <ID> : <TYPE> = <EXP>;```
<<<<<<< HEAD
<<<<<<< HEAD
| Structure expresion | ```<ID>(<EXP>, ...)```
| Function expresion | ```<ID>(<EXP>, ...)```
| Data expresion | ```<ID> : <TYPE>(<EXP>, ...)```
=======
>>>>>>> ebb9246 (Corrections)
=======
>>>>>>> 958816bb3b7e1c087402d4150c95b66b102d2bfb

### Example code

``` txt
// Point struct
struct Point (
    x : Float,
    y : Float
);

// Creation function
funct CreatePoint ( x : Float, y : Float ) 
: Point {
    return Point(x, y);
}

// Static data
data Origin : Point = Point(0.0, 0.0);

// Main function
funct Main ( args : String[] ) 
: Int {
    
    data point : Point = CreatePoint(0.0, 0.0);

    return 0;
}
```
