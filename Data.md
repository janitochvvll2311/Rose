# Data

* [Index](./Index.md)

## Declaration

* ```data ID ;``` Without type
* ```data ID ( ID : TYPE , ... ) ;``` With anonymus type
* ```data ID : TYPE ;``` With named type

## Definition

* ```data ID ( ID : TYPE = EXP, ... ) ;``` With members in-place
* ```data ID ( ID = EXP , ... ) ;``` With members in-place (inferred types)
* ```data ID ( ID : TYPE, ... ) = ( EXP, ... ) ;``` With members out-place
* ```data ID ( ID , ... ) = ( EXP , ... ) ;``` With members out-place (inferred types)
* ```data ID : TYPE ( EXP , ... ) ;``` With explicit type in-place constructor
* ```data ID : TYPE { ... } ;``` With explicit type in-place back code
* ```data ID : TYPE = EXP ;``` With explicit type expression
* ```data ID = EXP ;``` With inferred type expression

## Specials 1

* ```data ( ID : TYPE = EXP , ... ) ;``` Multiple data in-place assignment
* ```data ( ID = EXP , ... ) ;``` Multiple data in-place assignment (inferred types)
* ```data ( ID : TYPE , ... ) = ( EXP , ... ) ;``` Multiple data out-place assignment
* ```data ( ID , ... ) = ( EXP , ... ) ;``` Multiple data out-place assignment (inferred types)
* ```data ( ID : TYPE , ... ) = EXP ;``` Data deconstructor
* ```data ( ID , ... ) = EXP ;``` Data deconstructor (inferred types)

## Specials 2

* ```data ID ( EXP , ... ) ;``` Unnamed member in-place constructor
* ```data ID ( TYPE , ... ) = ( EXP , ... ) ;``` Unnamed member out-place constructor
* ```data ID ( TYPE , ... ) = EXP ;``` Unnamed member out-place deconstructor

## Usage

* ```ID . ID``` Named member access
* ```ID . INDEX``` Unnamed member access
