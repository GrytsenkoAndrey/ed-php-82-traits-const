# ed-php-82-traits-const

## Constants in Traits in PHP8.2

The “Constants in Traits” RFC was published on June 21st and is already available to the general public in the newest PHP 8.2:

```
<?php

// @see https://3v4l.org/fco7u

trait Foo {
    public const BAR = 'PHP';
}

class A {
    use Foo;
}

$a = new A();

echo $a::BAR;

// prints PHP
```

The voting phase was most controversial, having 28 votes for “yay” and 12 votes against — only 2 votes over the required passing threshold.

With 40 votes in total, the 2/3 majority of the core member squad is required for functionality to be accepted. One has to love democracy, right?

The externals.io discussions are always super interesting and informative. You might want to read it as well to know the point of view of the core members being against the feature.
