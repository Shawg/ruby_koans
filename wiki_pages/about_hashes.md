# Learning About Hash
A hash is a collection of key-value pairs. Each key corresponds to a particular value, and the key can be any kind of object.  
If there was a house with three locked doors, where each door could only be opened by a certain key and behind each door was a pile of cash, a key will only allow you to access the corresponding amount of cash that lies behind the door that it unlocks. Similarly, in a hash, a key will only allow you to access the element that it corresponds to.
```Ruby
hash_example = { 7 => 35, "c" => 2, "a" => 1 }
```  
In the example above, we can see that there are 3 key-value pairs: the key 7 which corresponds to the value 35, the key "c" which corresponds to 2, and the key "a" which corresponds to 1.  
So in the above hash, how do we access the value 2?
All we have to do is know which key the value 2 corresponds to:
```Ruby
hash_example["c"]
```  
hash_example["c"] will give you the value 2.
As you can see, a hash is similar to an array except that indexing is done via arbitrary keys of any object type, not an integer index.

For more information on Hash, check out [http://www.ruby-doc.org/core-1.9.3/Hash.html](http://www.ruby-doc.org/core-1.9.3/Hash.html)
