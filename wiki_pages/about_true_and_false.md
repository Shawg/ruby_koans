rning About True and False
The idea of something being true or false is extremely important in programming, and thus ruby.
They are what allows a control statement like
```ruby
if foo
    # Do something
end
```
to work! In order for you to do something in an if statement, foo must be true. But how can we find out what is and what isn't true.

Well in ruby true and false aren't just reserved keywords, they are a part of their own class, we can test this in irb as shown below.
```ruby
irb(main):001:0> true.class
=> TrueClass
irb(main):002:0> false.class
=> FalseClass
irb(main):003:0> foo = TrueClass.new
NoMethodError: undefined method `new' for TrueClass:Class
    from (irb):3
    from /usr/bin/irb:12:in `<main>'
irb(main):004:0> 
```
So we know that true and false are a part of their own class, and at irb(main):003 we showed that you can't create a new true or false object, but does this mean that true and false are the only objects that can be true or false? We can write a simple function to test this!
```ruby
def true_or_false( condition )
    if condition
        :true
     else
        :false
     end
end
```
We can use this function to test different types of conditions in order to find out if ture and false are the only things that can be true or false
As expected true returns true, and false returns false
```ruby
irb(main):008:0> true_or_false(true)
=> :true
irb(main):009:0> true_or_false(false)
=> :false
```
But you should test other conditions, strings! integers!
```ruby
irb(main):010:0> true_or_false(19)
=> :true
irb(main):011:0> true_or_false("Hello")
=> :true
```
You can see that everything is treated as true. Well, almost everything...
```ruby
irb(main):012:0> true_or_false(nil)
=> :false
```
You can see that nil is treated as false.
So knowing all of this, go ahead and complete about_true_and_false!

                                                   
