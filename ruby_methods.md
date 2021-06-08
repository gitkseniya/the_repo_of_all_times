### `string` methods
* `.capitalize`
* `.upcase`  
* `.downcase`
* `.reverse ` 
* `.sub`("t", "k")  
* .sub("tick","clock")
* `.gsub`("e","*")
* .gsub(/[aeiou]/,"")
* .greeting`.chomp`("!") // removes ""
* `.strip` - removes spaces and new lines
* `.length` // counts number of characters
* `.size` // does the same
* `.chop` // deletes the last character
* `.chomp` // deletes the last character or \n
* `.count`("o") // counts the number of "o"
* .count("aeiou") // counts all vowels
* `.include?`("llo")
* `.concat` // greeting.concat(" ", name) => greeting + " " + name
* `.delete` "!" // "Hello!!" => "Hello"

## integers & floats
* `.to_f` // unlucky / lucky.to_f => 1.8571428571428572
* `%` // modulo // 13 % 7 => 6
* `.even?` 
* `.round` // 3.14 = > 3
* .round(1) // to the 1st decimal
* `.floor` // 4.9999999999999.floor # => 4
* `.ceil` // 4.0000000000001.ceil  # => 5
* `.div(3)` // number can be divided by 3

### methods for `arrays.rb`
* array[1] // acesses second element in array
* array[-1] // last element
* `.count` // counts number of elements in array
* world_cup `<<` "Brazil" // adds this element to the end of array
* world_cup `<+=` "Brazil" // same
* `.pop` // remove last item from the array
* `.include?`
* `.shift`
* `.unshift` ("") // add this item to the beginning of the array
* teams[1..-1]// returns an array without 1st element
* `.compact` // removes nils from the array
* `.flatten` // removes nesting [[ [] [] ]] => []
* `.rotate`(2) // rotates two spots to the left
* .rotate(-1) // rotates one spot to the right
* `.delete`("y") // deletes "" from the array
* `.insert`(1, "dresser") // what index to insert to, and what
* `.join`(", ") // ["Sara, "Peter"]  => ["Sara, Peter]
* `.reverse`
* `.push`



### methods for `hashes.rb`

* `new(default)` - this version of .new gives the hash default values
* `[]`
* `[]=`
* `delete`
* `keys`
* `values`
* `length`/`size`

* `empty = {}` // assert.equal ({}), ...
*  empty = {:not_found `=> 0`} // create a key with a default value 0
* format:     ages = {"ben" => 4, "kelly" => 6}
* format2:    ages = {"ben": 4, "kelly": 6} // code runs faster, strings are compared by character, symbols - by the id
* grapes = books["John Steinbeck"] // returns a value to a key

### IC 
* setup
    - setup class
    - setup test 
    - test helper
