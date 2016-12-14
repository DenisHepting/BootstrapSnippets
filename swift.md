#Swift 


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


