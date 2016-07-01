# JavaScript

### General

- 2 spaces for consitency with HTML/CSS
  - this is important especially when using [jsx syntax](https://facebook.github.io/react/docs/jsx-in-depth.html)

- Soft 80 character line limit, with a hard 100 character line limit

  - Try avoid going over 80, but never go over 100

- anything declared using var should be in lowerCamelCase

  ```javascript
  var helloWorld;
  ```

- classes/constructors should be UpperCamelCase

  ```javascript
  helloWorld = new HelloWorld();
  ```

- constants should be all uppercase wtih and _ between workds

  ```javascript
  const HELLO_WORLD = "hello world!";
  ```

- For now there should be a colon at the end of every line, I might revoke this
rule in the future, but I haven't quite decided yet.

- 100% test coverage
  - if something isn't covered  there should be a document reason to why

- As much of the code as possible should be separated out in function so that
other developers can easily use code.

- Variable declaration includes a "var" for each variable

  Example:
  ```javascript
  var hello;
  var world;
  var good;
  var bye;
  ```

  not
  ```javascript
  var hello,
      world,
      good,
      bye;
  ```

- space between equal signs when declaring a variable

  ```javascript
  var x = 10;
  ```

  not:

  ```javascript
  var x=10;
  ```

- Good logical line breaks it's hard to have too much spacing.

  Example:
  ```javascript
    function getName(user){

      return user.name;

    }
  ```
  
  or

  ```javascript
    if(user){

      return user.name;

    }
  ```

  There should be at least one break for eaach if statement, and function 
  dclaration. It makes code much easier to read, you double space your english
  papers why not your code?

  Functions should also be between 10 and 20 lines, it's better to keep them
  small it gives the reader a much better understanding of what's going on. This
  is not a hard limit, so use your best judgment.


### Commenting

Commenting should be done frequently, it's hard to over comment. Every function
class and constuctor unless it's private then use your best judgment should have
a @desc, @param, and @return tags.

example:

```javascript
  /**
   * @desc Fetches the user name
   * @param {Object} user - the user object who's name is being fetched
   * @return {string} - the user's name
   */
  function getName(user){

    return user.name;

  }
```

These tags will be used to automatically generate documentation using either
[jsdoc](http://usejsdoc.org/) or [esdoc](https://esdoc.org/)


- All block comments should have the "/**" with the "/" line up with the current
  block indentation, and then the "*"s should line up with the first star, so
  one space over from the current block indentation. There should hen be one space
  after the star and before the first character
