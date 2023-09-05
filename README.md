# PHP CodeSniffer rules for Laravel coding style (PSR-2 variant)

[![MIT Licensed](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE.md)
[![PR friendly repository](https://img.shields.io/badge/Pull--Request-are%20welcome!-ff69b4)](/compare)
![Follow Fossbarrow on Twitter](https://img.shields.io/twitter/follow/fossbarrow?style=social)

> Authored by fossbarrow IO


[php codesniffer ruleset](https://github.com/squizlabs/PHP_CodeSniffer/wiki/Annotated-Ruleset) for laravel projects.

## Requirements

- https://github.com/squizlabs/PHP_CodeSniffer

## Table of contents

- [How to install](#install)
    - [Enabling the rules](#enabling-the-rules)
    - [Sniffing code](#sniffing-code)
    - [Sniffing code in PHPStorm](#sniffing-code-in-phpstorm)
- [License](#license)
- [Contributing](#contributing)
- [Credits](#credits)

## Installation
Install the ruleset by

1. Copy the `phpcs.xml` file into your project root with phpcs installed.

## Usage

### Enabling the rules

> Only neccesary if you installed as a package using composer!

Add it to your project `phpcs.xml` or `phpcs.xml.dist` ruleset:

```xml
<?xml version="1.0"?>
<ruleset>
    <arg name="basepath" value="."/>

    <file>./app</file>
    <file>./config</file>
    <file>./resources</file>
    <file>./routes</file>
    <file>./tests</file>

    <rule ref="./vendor/fossbarrow/laravel-phpcs/phpcs.xml"/>
</ruleset>
```

### Sniffing code
Use php CodeSniffer commands, pointed towards your xml file, to sniff the code
using the new ruleset.

> vendor/bin/phpcs
> vendor/bin/phpcbf

#### Sniffing code in PHPStorm

See [PHP Code Sniffer in PhpStorm](https://confluence.jetbrains.com/display/PhpStorm/PHP+Code+Sniffer+in+PhpStorm) on how to set up CodeSniffer in PHPStorm.

--------------------------------------------------------------------------------


## Contributing

All changes that makes the sniffer more accurate towards _Laravel_'s coding standard
is always highly appreciated and welcome. 

Please see [CONTRIBUTING](docs/CONTRIBUTING.md) for more details.

## Credits

- [PatricNox](https://github.com/PatricNox)
- [All Contributors](../../contributors)

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
