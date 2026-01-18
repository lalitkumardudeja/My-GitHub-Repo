# My-GitHub-Repo
Welcome to a beginner-friendly repository designed to help you learn **Git**, **GitHub**, and **WordPress development**. This project includes basic examples and tutorials, including a Hello World plugin for WordPress, and instructions for how to fork, clone, and make contributions. It's perfect for practicing version control and contributing to open-source projects.

## What You Can Do Here:
- **Fork** the repository to create your own copy.
- **Clone** it to your local machine and explore the code.
- **Make Changes**: Feel free to modify the existing code, add new features, or improve the documentation.
- **Submit a Pull Request**: If you make any changes, you can submit a pull request to contribute them back to this repository.

## Example Code: Hello World WordPress Plugin

This simple WordPress plugin adds a "Hello, World!" message to the footer of your WordPress site. It’s a great starting point for practicing WordPress plugin development and understanding how plugins work.

### Plugin Code:
Create a PHP file named `hello-world-plugin.php` and add the following code to it:

```php
<?php
/*
Plugin Name: Hello World Plugin
Description: A simple WordPress plugin that displays "Hello, World!" in the footer.
Version: 1.0
Author: Lalit Kumar Dudeja
*/

// Function to display "Hello, World!" in the footer
function hello_world_footer_message() {
    echo '<p>Hello, World! Welcome to my WordPress site.</p>';
}

// Hook the function to the WordPress footer
add_action('wp_footer', 'hello_world_footer_message');
