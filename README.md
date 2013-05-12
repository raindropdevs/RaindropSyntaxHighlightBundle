#SyntaxHighlightBundle

####This bundle includes Code Mirror js library for textarea code highlighting
Documentation and examples are available at [Code Mirror Official  Website](http://codemirror.net/)


See a basic usage [here](https://github.com/raindropdevs/RaindropTwigLoaderBundle/blob/master/Resources/public/js/templateAdmin.js)

A twig highlighter mode is into roadmap.

===

### **INSTALLATION**:

First add the dependency to your `composer.json` file:

    "require": {
        ...
        "raindrop/syntax-highlight-bundle": "dev-master"
    },

Then install the bundle with the command:

    php composer.phar update

Enable the bundle in your application kernel:

``` php
<?php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new Raindrop\SyntaxHighlightBundle\RaindropSyntaxHighlightBundle(),
    );
}
```

Now install assets:

    php app/console assets:install [--symlink]
