#Wordpress Snippets Sublime


**wp:Img** -> Defines normal Image Wordpress


```php

<?php if(!empty($section6_img)) : ?> 
    <img class="img-responsive" src="<?php echo $section6_img['url']; ?>" alt="<?php echo $section6_img['alt']; ?>">
<?php endif; ?>

<?php echo ?>

```



**wp:CSSImg** -> Defines CSS-Background in WP-PhP
<?php if(!empty($myVar)) : ?>
        style="background-image: url('<?php echo $myVar['url']; ?>');">
<?php endif; ?>


**php:Echo** -> Gives PHP for simple-text echo back 

