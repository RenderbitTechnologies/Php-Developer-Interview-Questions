# Php Developer Interview Questions

A nice set of non-riddle, real world questions which should result in a well formed oppinoin of a developers experience in PHP and full stack web development.


## - Explain what PHP 'safe mode' means when writing a PHP script.
Here we are looking for the developer to raise the main point that PHP's safe mode prevents scripts from modifying PHP configuration anywhere other than the php.ini file. This is a good question to guage how familiar they really are with PHP rules and it's legacy, usually the bedroom developers don't get this one.

## - What is the difference between SELF::foo() and $this->foo()
This is a good question for a few reasons. Firstly the developer should recoginse that SELF is calling a static function while $this is calling a member function. They should also identify that SELF is a reference to a class while $this is a reference to an object. This an important distinction in OO programming and especially in PHP entity driven applications.

## - What are the latest PHP versions?
Does this person really know PHP? Or do they just use tools and systems written in PHP? The developer should identify PHP 7.1 and PHP 5.6 as the latest versions. CMS monkeys don't usually get this one.

## - What connects the web server (apache or nginx) with PHP and what 2 ways can these communicate?
Has this person every configured PHP before? Of course here we're looking for them to identify our hero, php-fpm and either a TCP connection or a socket connection between them. Bonus points for touting TCP as the better option.

## - How would we reliably get a users IP address in a PHP script?
Here we are obviously looking for them to reference the $_SERVER['REMOTE_ADDR'] global. Given the widespread use of load balancers it's not unreasonable to expect a devleoper to also reference $_SERVER['X-FORWARDED-FOR'].

## - What is a PHP trait and why are they important?
In this question we're looking for the developer to tell us that PHP cannot handle multi-inheritance and that traits are the way around this. They allow us to reuse code in multiple entities while leaving our single inheritance options available.

## - What does 'Warning: Cannot modify header information – headers already sent' mean? How do we avoid it in our classes?
This is a common error which occurs when whitespace exists before an opening PHP tag or between two sets of PHP code. This can generally be avoided by not closing php tags within our classes.
