rning About Nil
nil represents a non-existent object, or nothing.
Unlike NULL in other languages, nil is an object and is part of the nil class.
If you check out the [documentation for the nil class](http://ruby-doc.org/core-1.9.3/NilClass.html#method-i-nil-3F), you can see that nil has a few methods defined on it, such as nil?().

The method nil?() returns true only if the object that is calling it is nil.  
So if we want to test if an object is nil, we can use  
```ruby
obj.nil?
```  
However, we can also test if an object is nil by using  
```ruby
obj == nil
```  
Using either way works, but using obj.nil? is the better option because it is easier to read than obj == nil.

A few other examples of methods defined on nil are  
```ruby
nil.to_s
```
and
```ruby
nil.inspect
```  
nil.to_s will return the empty string, while nil.inspect will return the string "nil".

