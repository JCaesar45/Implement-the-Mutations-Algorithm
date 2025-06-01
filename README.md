````markdown
# Mutation Algorithm

## Project Description
This project implements a function named `mutation` that determines if all the letters in the second string of an array are present in the first string, ignoring case sensitivity.

The function helps verify whether one string "contains" all characters of another string, which can be useful in various string validation or comparison tasks.

---

## Features

- Case-insensitive comparison between two strings
- Returns `true` if all letters in the second string are present in the first string
- Returns `false` otherwise

---

## Function Signature

```javascript
function mutation(arr) {
  // implementation here
}
```

### Parameters:

* `arr` (Array): An array of two strings `[string1, string2]`

### Returns:

* `Boolean`: `true` if every character in `string2` is found in `string1` (case-insensitive), otherwise `false`.

---

## Examples

```javascript
mutation(["hello", "Hello"]); // true
mutation(["hello", "hey"]);   // false
mutation(["Alien", "line"]);  // true
mutation(["floor", "for"]);   // true
mutation(["hello", "neo"]);   // false
```

---

## How to Run

1. Copy the `mutation` function code into a JavaScript environment (browser console, Node.js, or an online editor).
2. Call the function with your desired inputs as shown in the examples.
3. Observe the boolean output in the console.

---

## Code Implementation

```javascript
function mutation(arr) {
  let first = arr[0].toLowerCase();
  let second = arr[1].toLowerCase();

  for (let char of second) {
    if (!first.includes(char)) {
      return false;
    }
  }
  return true;
}
```

---

## License

This project is open source and free to use.

---
