
### 🚧 Problem: Word Problem

**Description**:  
There is a bus moving in the city which takes and drops some people at each bus stop.
You are provided with a list (or array) of integer pairs. Elements of each pair represent the number of people that get on the bus (the first item) and the number of people that get off the bus (the second item) at a bus stop.
Your task is to return the number of people who are still on the bus after the last bus stop (after the last array). Even though it is the last bus stop, the bus might not be empty and some people might still be inside the bus, they are probably sleeping there :D
Take a look on the test cases.
Please keep in mind that the test cases ensure that the number of people in the bus is always >= 0. So the returned integer can't be negative.
The second value in the first pair in the array is 0, since the bus is empty in the first bus stop.

**Input**:
```txt

// array_sum = returns the sum of all the values in the array.
// array_column = returns the values from a single column in the input array.

function number($bus_stops) {
  return array_sum(array_column($bus_stops, 0)) - array_sum(array_column($bus_stops, 1));
}
```

### 🚧 Problem: Word Problem

**Description**:  
You are going to be given a non-empty string. Your job is to return the middle character(s) of the string.

- If the string's length is odd, return the middle character.
- If the string's length is even, return the middle 2 characters.

**Example**:
```txt
"test" --> "es"
"testing" --> "t"
"middle" --> "dd"
"A" --> "A"
```

**Solutions**:
```txt

// strlen = returns the length of a string.
// substr = returns a part of a string.

function getMiddle($text) {
  $length = strlen($text);
  return substr($text, ($length - 1) / 2, $length % 2 == 0 ? 2 : 1);
}
```

### 🚧 Problem: Word Problem

**Description**:  
You are going to be given a non-empty string. Your job is to return the middle character(s) of the string.

- If the string's length is odd, return the middle character.
- If the string's length is even, return the middle 2 characters.

**Example**:
```txt
"test" --> "es"
"testing" --> "t"
"middle" --> "dd"
"A" --> "A"
```

**Solutions**:
```txt

// strlen = returns the length of a string.
// substr = returns a part of a string.

function getMiddle($text) {
  $length = strlen($text);
  return substr($text, ($length - 1) / 2, $length % 2 == 0 ? 2 : 1);
}
```

### 🚧 Problem: Word Problem

**Description**:  
Implement a function that computes the difference between two lists. The function should remove all occurrences of elements from the first list (a) that are present in the second list (b). The order of elements in the first list should be preserved in the result.

**Example**:
```txt
If a = [1, 2] and b = [1], the result should be [2].
If a = [1, 2, 2, 2, 3] and b = [2], the result should be [1, 3].
```

**Solutions**:
```txt

// array_values = returns an array containing all the values of an array.
// array_diff = compares the values of two (or more) arrays, and returns the differences.

function arrayDiff($a, $b) {
  return array_values(array_diff($a, $b));
}
```

### 🚧 Problem: Word Problem

**Description**:  
Implement a function that computes the difference between two lists. The function should remove all occurrences of elements from the first list (a) that are present in the second list (b). The order of elements in the first list should be preserved in the result.

**Example**:
```txt
If a = [1, 2] and b = [1], the result should be [2].
If a = [1, 2, 2, 2, 3] and b = [2], the result should be [1, 3].
```

**Solutions**:
```txt

// min =  returns the lowest value in an array, or the lowest value of several specified values.
// array_map = sends each value of an array to a user-made function, and returns an array with new values, given by the user-made function.
// explode = breaks a string into an array.

function findShort($str){
   return min(array_map('strlen', (explode(' ', $str))));
}
```
