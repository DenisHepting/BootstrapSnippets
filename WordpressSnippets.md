#Wordpress Snippets Sublime


**wp:Img** -> Defines normal Image Wordpress

```php
<?php if(!empty($yourVar_img)) : ?> 
   <img class="img-responsive" src="<?php echo $yourVar_img['url']; ?>" alt="<?php echo $yourVar_img['alt']; ?>">
<?php endif; ?>
```

**wp:CSSImg** -> Defines CSS-Background in WP-PhP
```php
<?php if(!empty($myVar)) : ?>
        style="background-image: url('<?php echo $myVar['url']; ?>');">
<?php endif; ?>
```

**php:Echo** -> Gives PHP for simple-text echo back 

