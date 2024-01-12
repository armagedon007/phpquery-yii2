# phpQuery

phpQuery is a PHP library that enables you to parse HTML and manipulate the DOM using jQuery-like syntax. This repository aims to create a PHP 8.x ready version derived from the original code available in the [Google Code Archive](https://code.google.com/archive/p/phpquery/).

Fork https://github.com/php-query/php-query

## License

This project is based on the original code released under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contribution Guidelines

We welcome and appreciate contributions from the community. If you'd like to contribute, please follow these guidelines:

- Fork the repository
- Create a new branch for your feature or bug fix
- Commit your changes and push your branch to your fork
- Open a pull request with a clear description of your changes

We appreciate bug reports, feature requests, and any other form of contribution. Your help makes this project better for everyone.

## Installation

To use phpQuery in your project, you can install it via Composer:

```bash
composer require aramgedon007/phpquery-yii2
```

## Usage

Here's a simple example of how you can use phpQuery in your PHP code:

```php
use phpQuery;

// Create a new phpQuery object
$html = '<div><p>Hello, <span>world!</span></p></div>';
$doc = phpQuery::newDocument($html);

// Manipulate the DOM using jQuery-like syntax
$text = $doc['div p span']->text(); // Retrieve the text content
echo $text; // Output: world!
```

