WordPress Console
===============

This script will provide an interactive console similar to `rails console` if
you're familiar with Ruby on Rails.

In order to use this, you need to have php-cli installed with readline support.

Requirements
------------

PHP >= 4.2.3 w/ libreadline support

Installation
------------

1. Download the `wp-console` file into your WordPress root.
2. Make the `wp-console` script executable with `chmod +x wp-console`.

Usage
-----

To run the console, simply execute `./wp-console` from the root of your
WordPress project. This will give you an interactive prompt where you can
experiment with WordPress code:

~~~~
franklin@server:/var/www$ ./wp-console
Interactive shell

php > $post = get_post(1);
php > print_r($post);
WP_Post Object
(
    [ID] => 1
    [post_author] => 1
    [post_date] => 2013-03-26 03:00:48
    [post_date_gmt] => 2013-03-26 03:00:48
    [post_content] => Welcome to WordPress. This is your first post. Edit or delete it, then start blogging!
    [post_title] => Hello world!
    [post_excerpt] => 
    [post_status] => trash
    [comment_status] => open
    [ping_status] => open
    [post_password] => 
    [post_name] => hello-world
    [to_ping] => 
    [pinged] => 
    [post_modified] => 2013-03-26 04:26:03
    [post_modified_gmt] => 2013-03-26 04:26:03
    [post_content_filtered] => 
    [post_parent] => 0
    [guid] => http://franklinstrube.local/wordpress/?p=1
    [menu_order] => 0
    [post_type] => post
    [post_mime_type] => 
    [comment_count] => 1
    [filter] => raw
)
~~~~
