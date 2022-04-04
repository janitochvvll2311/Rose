# Namespace

* [Index](./Index.md)

## Definition

* ```namespace ID ;``` Whole file namespace
* ```namespace ID . ID ;``` Whole file inline-nested namespace
* ```namespace ID { ... } ;``` Scoped namespace
* ```namespace ID . ID { ... } ;``` Scoped inline-nested namespace
* ```namespace ID { namespace ID { ... } } ;``` Scoped nested namespace

## Usage

* ```ID . TYPE``` Where ID is a namespace ID  
* ```ID . ID . TYPE``` Nested namespace  
* ```ID . { ... }``` Access code (Where ID is a namespace ID)
