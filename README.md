# sz-wp-boilerplate
_Very_ stripped-down boilerplate for WordPress theme development.

## Features
- SASS directory and base files, as well as `sz-navbar` for pure-CSS responsive navbar
- inc directory and base customizer, helper-functions, and register-menus scripts
- template_parts directory with base article.php part template
- functions.php queues custom CSS, FontAwesome, Google Fonts
- templates:
    - header.php with navbar
    - index.php displaying all posts
    - single.php
    - footer.php

## Usage
1. Search for all instances of `sz-template-` and `sz_template_` and replace with your own prefix. Or don't, if you want to just keep them.

    Note: There are a few instances of `sz-` without `template` afterwards that should be left in; these are things like helper functions and libraries that I've written and included.
    
2. In functions.php, replace the url in `wp_enqueue_style('google_fonts', ...)` with your own Google Fonts url.