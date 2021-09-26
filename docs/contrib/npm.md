<!-- DO NOT EDIT THIS FILE! -->
<!-- Instead edit contrib/npm.php -->
<!-- Then run bin/docgen -->

# npm

[Source](/contrib/npm.php)


## Installing

Add to your _deploy.php_

```php
require 'contrib/npm.php';
```

## Configuration

- `bin/npm` *(optional)*: set npm binary, automatically detected otherwise.

## Usage

```php
after('deploy:update_code', 'npm:install');
```





## Tasks

### npm:install
[Source](https://github.com/deployphp/deployer/blob/master/contrib/npm.php#L30)

Install npm packages.

In there is a {{previous_release}}, node_modules will be copied from it before installing deps.

