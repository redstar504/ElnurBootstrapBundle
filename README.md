ElnurBootstrapBundle
====================

This bundle provides unobtrusive support for Bootstrap 3. By “unobtrusive” I mean that it doesn't force some particular
styling unless you explicitly tell it to. For example, by default, forms get the default Bootstrap styling — not
horizontal or something else like that.

Installation
------------

The bundle assumes that you install Bootstrap yourself by whatever means you like — be it a Composer package or via
Bower.

To install the bundle itself, add the following to your `composer.json`:

    {
        "require": {
            "elnur/bootstrap-bundle": "~0.1@dev"
        }
    }

And tell Composer to install the bundle:

    $ php composer.phar update elnur/bootstrap-bundle

Then enable the bundle by adding the following to your `AppKernel.php`:

    public function registerBundles()
    {
        $bundles = array(
            // ...
            new Elnur\Bundle\BootstrapBundle\ElnurBootstrapBundle,
        );

        // ...
    }