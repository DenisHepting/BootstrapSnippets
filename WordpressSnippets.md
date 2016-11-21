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