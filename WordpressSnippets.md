#Wordpress Snippets Sublime 3


**wp:Img** -> Defines normal image Wordpress

```php
<?php if(!empty($yourVar_img)) : ?> 
   <img class="img-responsive" src="<?php echo $yourVar_img['url']; ?>" alt="<?php echo $yourVar_img['alt']; ?>">
<?php endif; ?>
```

**wp:CSSImg** -> Defines CSS-Background in WP-PHP, insert into DIV 
```php
<?php if(!empty($yourVar)) : ?>
        style="background-image: url('<?php echo $yourVar['url']; ?>');">
<?php endif; ?>
```

**php:Echo** -> Gives PHP for simple-text echo back 
```php
<?php echo $yourVar ?>
```

```swift
struct Coordinates{
var a = 10 
var b = 20

init(a: Int, b: Int){
   self.a = a
   self.b = b
}


}
```

**Oh thats Interessting my friend***
**I just added that to my local files ***

Small scale Shopping App Logic

```swift
	
	// Shirt Struct
struct TShirt{
    var color: String
    var prize: Int
    var size: String
    
    init(color: String, prize: Int, size: String) {
        self.color = color
        self.prize = prize
        self.size = size
    }
}
// Adress Struct
struct Adress{
    var street: String
    var city: String
    var zipCode: Int
    
    init(street: String, city: String, zipCode: Int){
        self.street = street
        self.city = city
        self.zipCode = zipCode
    }
}

// Shopping Cart Class
class ShoppingCart{
    var shirts = [TShirt]()
    var totalPrice = 0
    var shippingAdress: Adress
    
    init(shippingAdress: Adress) {
        self.shippingAdress = shippingAdress
    }
    
    func calcTotalPrice(){
        for i in 0...shirts.count-1{
         totalPrice = totalPrice + shirts[i].prize
        }
    }
    
    func printCart() {
        print("In your cart are \(shirts.count) shirts. And the total Price is \(totalPrice)")
    }
}

// User Class
class User{
    var name: String
    var email: String
    var shoppingCart: ShoppingCart
    
    init(name: String, email: String, shoppingCart: ShoppingCart) {
        self.name = name
        self.email = email
        self.shoppingCart = shoppingCart
    }
}

```


Header-Search Animation
```CSS
 
#header-search {
	position: absolute;
	width: 100%;
	height: 100%;
	color: #fff;
	-webkit-transition-property: all;
	transition-property: all;
	transition-duration:.3s;
	-webkit-transition-duration:.3s;
	pointer-events: none;
	left: 0;
	z-index: 199;
	top: -100%;
	background: #000;
}

#header-search.open {
	top: 0;
	opacity: 1;
	pointer-events: auto;
	
}


.split-header #site-header .inside {
	text-align: center !important;
}

.split-header .logo, .split-header .logo  {
	margin: 0 auto !important;
	float: none;
	position: absolute;
	width: 100%;
}

.inline-header .logo, .split-header .logo {
	height: 90px;
}

.sticky .logo {
	height: 60px !important;
}

.logo img {
	transition-property: all;
	-webkit-transition: 0.3s ease;
		    transition: 0.3s ease;
}
```

Class inheritance and overriding class methods 

```swift
struct Grades{
    var points: Int
    var credits: Int
    var letter: String
    
    init(points: Int, credits: Int, letter: String) {
        self.points = points
        self.credits = credits
        self.letter = letter
    }
}

class Person{
    var firstName: String
    var lastName: String
    
    init(firstName: String, lastName: String) {
        self.firstName = firstName
        self.lastName = lastName
    }
    
 
}

class Student : Person{
    var grades: [Grades] = []
    
    func printIt(){
        print(firstName + " " + lastName)
        print(grades)
    }
    
    func recordGrade(grade:Grades){
        grades.append(grade)
    }
    
}

class AlthleteStudent : Student{
    var missedCourses: [Grades] = []

    
    override func recordGrade(grade: Grades) {
        super.recordGrade(grade: grade)
        
        if grade.letter == "F"{
            missedCourses.append(grade)
        }
    }
    
    func checkForKickout() -> Bool{
        return missedCourses.count < 3
    }
}

```
