#Swift 

##What to know
 + **variables** ✅
 + **constants** ✅
 + **operators** ✅
 + **if, switch** ✅
 + **for, while, repeat** ✅ (repeat review)
 + **ranges** ✅
 + **break, continue** ❌❓
 + **tenery condition operator** ✅ (review) 
 + **functions** ✅
 + **arrays** ✅
 + **sets** ✅ (review set operation)
 + **dictionaries** ✅
 + **higher order functions (map, sort, filter)** ✅
 + **closures** ❌❓
 + **optionals** ❌❓
 + **structs** ✅
 + **classes** ✅
 + **advanced classes (inheritance)** ✅
 + **enumeration**


##Variables 

Swift has a so called type inference with which it is able to recognize the type you use as a variable. If you want to make sure that a certain type is 
not accidentally used as another, or overwritten declare it right away. Swift is type safe, so it doesn't allow you to overwrite a type you already used. 


```swift
// define the type
var typeReference: Int = 0 

//INT 
var x = 10 

//DOUBLE 
var y = 54.0

//STRING
var firstName = "Peter"

//BOOL 
var isPlaying = true 

```


##Constants

If you don´t plan to change the value of your variable, or a value should never changed be accidentally changed, cause it is a constant, make it a let (constant)

```swift
//Constants are declared as let 

let pi = 3.14

let vowel = "a"

let adminName = "Juergen"
```


##Operators

The operators are pretty much same like in all the other programming languages

AND &&
OR ||
Smaller <=
Bigger >=
Equals == 

You are also able to chain them like in every other languages

(a < x && z > b ) || 10 == currentValue

##


##Use functions as input parameter

```swift

// use a function as input parameter like that (functionInput: (Int, Int) -> Int)

func addTwoValues(first: Int, second: Int)->Int{
    return first + second
}

func funktionMitFunktion(mathcalculation: (Int, Int) -> Int, a: Int, b: Int)->Int{
    return mathcalculation(a,b)
}


funktionMitFunktion(mathcalculation: addTwoValues, a: 10, b: 10)

```



##Nested functions

```swift


func chooseStepFunction(backward: Bool) -> (Int) -> Int {
    // nested functions, stepping back or frontwards
    func stepForward(Input: Int) -> Int { return Input + 1 }
    func stepBackward(Input: Int) -> Int { return Input - 1 }
    // Tenery gives stepBackward if backward is false, else gives stepForward
    return backward ? stepBackward : stepForward
}

var currentValue = -10

let moveCloserToZero = chooseStepFunction(backward: currentValue > 0)

while currentValue != 0 {
    print("\(currentValue)")
    currentValue = moveCloserToZero(currentValue)
}



```


+**hello** adress.com

