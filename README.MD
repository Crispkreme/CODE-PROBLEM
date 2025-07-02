
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
$stop = [
    [10, 0],
    [3, 5],
    [5, 8],
];

function number(array $stop): int {
  
  $totalPeople = 0;
  
  foreach ($stop as $bus_stops) {
      $peopleOn = $bus_stops[0];
      $peopleOff = $bus_stops[1];
    
      $totalPeople = $totalPeople + $peopleOn - $peopleOff;
  }
  
  return $totalPeople;
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
$stop = [
    [10, 0],
    [3, 5],
    [5, 8],
];

function number(array $stop): int {
  
  $totalPeople = 0;
  
  foreach ($stop as $bus_stops) {
      $peopleOn = $bus_stops[0];
      $peopleOff = $bus_stops[1];
    
      $totalPeople = $totalPeople + $peopleOn - $peopleOff;
  }
  
  return $totalPeople;
}
```
