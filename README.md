Brainbits Fugue Icons Bundle
============================
This bundle provides the excellent fugue icon set from Yusuke Kamiyamane, which can be found at http://p.yusukekamiyamane.com/.

### Step 1: Download BrainbisFugueIconsBundle using composer

Add BrainbitsFugueIconsBundle in your composer.json:

```js
{
    "require": {
        "brainbits/fugue-icons-bundle": "*"
    }
}
```

Now tell composer to download the bundle by running the command:

``` bash
$ php composer.phar update brainbits/fugue-icons-bundle
```

Composer will install the bundle to your project's `vendor/brainbits` directory.

### Step 2: Enable the bundle

Enable the bundle in the kernel:

``` php
<?php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new Brainbits\FugueIconsBundle\BrainbitsFugueIconsBundle(),
    );
}
```

### Step 3: Install assets

This step is only necessary after adding, afterwards the assets will be installed 
on composer update.

``` bash
$ php app/console assets:install
```



