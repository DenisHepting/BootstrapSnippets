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
