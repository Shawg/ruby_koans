# Learning About Strings
A string is a sequence of characters used to represent text, such as "hello world". Strings are extremely important and are frequently involved in all kinds of operations, such as printing a message to your console, or reading from a text file.

In Ruby, strings can be initialized with double or single quotes.  
```ruby
string = "Hello, World"
string = 'Hello, World'
```  
Strings can also be quoted with different characters by using %.  
```ruby
string = %!flexible quotes can handle both ' and " characters!
``` 

We can also concatenate strings together using +.
```ruby
string = "Hello " + "World".
final_string = string + ". Hello"
```  
final_string would contain "Hello World. Hello"

However, if we want to modify an existing string, we can use + or <<.
```ruby
string = "Hi "
string += "Hi "
string << "Hi "
```  
string would now contain "Hi Hi Hi "

As an aside, we can also obtain the same string above by multiplying!
```ruby
string = "Hi"*3
```  

Another important concept of strings are substrings. A substring is a string that occurs in another string. For example, a substring of "Hello World" could be "Hello Wo". There are a few ways you can create substrings from strings (Check out [this link](http://www.ruby-doc.org/core-1.9.3/String.html#method-i-5B-5D) for other ways of creating substrings).
```ruby
a = "How's it going?"
a[6,3]
a[6..10]
```  

Both a[6,3] and a[6..10] would be equal to "it ". Note that the first character starts at 0 just like an array! Strings are often implemented as an array of characters. So, if we tried a[0], we would get the first character of the string a, which is 'H'.

There are many other important features of strings that you will see in about_strings such as variable interpolation and splitting.
Check out http://www.ruby-doc.org/core-1.9.3/String.html to learn more about the string class in Ruby!
