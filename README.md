# acf-json
Force ACF to store and load json for specific groups in a specific place, useful for plugins and themes which define their own ACF groups.

# Installing
```
composer require vena/acf-json
```

# Using
Assuming you're using composer's autoload, setup is simple.
```php
$acfJson = new \vena\AcfJson\Loader(
	[
		// Group IDs to store and load
		'group_61240bc1afe31',
		'group_612524d9ef624',
	],
	// Path under which to create acf-json folder
	// and store ACF's json for the groups
	__DIR__
);
```