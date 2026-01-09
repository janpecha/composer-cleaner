Victor The Cleaner for Composer
===============================

<a href="https://www.janpecha.cz/donate/"><img src="https://buymecoffee.intm.org/img/donate-banner.v1.svg" alt="Donate" height="100"></a>

This tool removes unnecessary files and directories from Composer vendor directory.

Forked from originally [dg/composer-cleaner](https://github.com/dg/composer-cleaner).

Installation
------------

```
composer require janpecha/composer-cleaner
```

Then simply use `composer update`.


Configuration
-------------

You can also specify paths to be ignored (ie they will not be deleted) via `composer.json`:

```js
{
	"extra": {
		"cleaner-ignore": {
			"slevomat/eet-client": [  // name of package
				"wsdl*"               // files or subdirectories, you can use wildcards `*` and `?`
			],

			"mpdf/mpdf": true         // ignores whole package
		}
	}
}
```
