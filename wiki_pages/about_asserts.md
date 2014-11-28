Assertions are the heart of Ruby Koans, as well as Test Driven Development.
In their simplest form, you can just assert something by using 

```ruby    
assert foo
```
and if foo is true, then you don't have a problem! But in the case that foo is false, you will get an error message and have to change whatever foo is to be true in order for the code to work.

We can use assertions to test the equality of two different things
```ruby 
assert foo == bar
```
this will tell us if foo and bar are equal. But we can do this in a better way!

```ruby
assert_equals foo, bar
```

This also tells us if foo and bar are equal, but using assert_equals makes the code a little bit easier for a human to read.

So knowing all of this, go ahead and complete about_asserts!

