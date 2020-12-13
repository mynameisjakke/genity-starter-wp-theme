Genity Starter Theme
===

This is a starter theme called `Genity Starter`, it's a team ment for speeding up the theme development for websites created by Genity... And create the most Awesome WP sites!

* This theme is based on a modern workflow with a pre-made CLI.
* Well documented templates (to be a bit future proof).
* Custom header implementation in `inc/custom-header.php`. 
* Custom template tags in `inc/template-tags.php`.
* Some smaller tweaks in the `inc/template-functions.php` that hopefully improve the experience.
* Full support from `WooCommerce` integration with hooks and so on in `inc/woocommerce.php`
* Licensed under GPLv2 or later. 
  

## Installation

### Requirements
`Genity starter` requires the following dependencies:
-  [Node.js](https://nodejs.org/)
-  [Composer](https://getcomposer.org/)

### Quick Start
Clone this repo, change its name to the desired theme name (like `Potato Theme`), and then you need to follow these six steps to replace the name in all the templates

1. Search for `'genity-starter'` (inside single quotations) to capture the text domain and replace with: `'potato-theme'`.

2. Search for `genity-starter_` to capture all the functions names and replace with: `potato-theme_`.

3. Search for `Text Domain: genity-starter` in `style.css` and replace with: `Text Domain: potato-theme`.

4. Search for <code>&nbsp;genity-starter</code> (with a space before it) to capture DocBlocks and replace with: <code>&nbsp;potato-theme</code>.

5. Search for `_genity-starter-` to capture prefixed handles and replace with: `potato-theme-`.

6. Search for `_GENITY-STARTER_` (in uppercase) to capture constants and replace with: `POTATO-THEME_`.

Then, update the stylesheet header in `style.css`, the links in `footer.php` with your own information and rename `genity-starter.pot` from `languages` folder to use the theme's slug. Next, update or delete this readme.

### Setup
To start using all the tools that come with `genity-starter` you need to install the necessary Node.js and Composer dependencies :

```sh

$ composer install

$ npm install

```

### Available CLI commands
`genity-starter` comes packed with CLI commands tailored for WordPress theme development :

*  `composer lint:wpcs` : checks all PHP files against [PHP Coding Standards](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/php/).

*  `composer lint:php` : checks all PHP files for syntax errors.

*  `composer make-pot` : generates a .pot file in the `languages/` directory.

*  `npm run compile:css` : compiles SASS files to css.

*  `npm run compile:rtl` : generates an RTL stylesheet.

*  `npm run watch` : watches all SASS files and recompiles them to css when they change.

*  `npm run lint:scss` : checks all SASS files against [CSS Coding Standards](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/css/).

*  `npm run lint:js` : checks all JavaScript files against [JavaScript Coding Standards](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/javascript/).

*  `npm run bundle` : generates a .zip archive for distribution, excluding development and system files.

Now you're ready to go! 