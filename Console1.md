# Essential JavaScript Console Methods for Professional Developers

## `console.log()`
- **Example:**
  ```javascript
  const num = 10;
  console.log("The value of num is:", num);
  ```
- **Explanation:** Used to print messages to the console. It can take multiple arguments and display them with proper formatting.

## `console.error()`
- **Example:**
  ```javascript
  const errorMessage = "Something went wrong!";
  console.error(errorMessage);
  ```
- **Explanation:** Outputs an error message to the console, typically in red color, indicating a critical error.

## `console.warn()`
- **Example:**
  ```javascript
  const warningMessage = "This action is not recommended.";
  console.warn(warningMessage);
  ```
- **Explanation:** Outputs a warning message to the console, typically in yellow color, indicating a non-critical issue.

## `console.info()`
- **Example:**
  ```javascript
  const infoMessage = "Information: User logged in successfully.";
  console.info(infoMessage);
  ```
- **Explanation:** Outputs an informational message to the console, typically in blue color, providing additional information.

## `console.debug()`
- **Example:**
  ```javascript
  const debugMessage = "Debugging information...";
  console.debug(debugMessage);
  ```
- **Explanation:** Outputs a debug message to the console, typically used for debugging purposes during development.

## `console.assert()`
- **Example:**
  ```javascript
  const condition = false;
  console.assert(condition, "Condition is not true!");
  ```
- **Explanation:** Checks if a specified condition is true. If not, it logs an error message to the console.

## `console.clear()`
- **Example:**
  ```javascript
  console.clear();
  ```
- **Explanation:** Clears the console of all previous messages and logs.

## `console.table()`
- **Example:**
  ```javascript
  const users = [
    { id: 1, name: "John", age: 30 },
    { id: 2, name: "Jane", age: 25 },
  ];
  console.table(users);
  ```
- **Explanation:** Displays tabular data in a table format in the console, making it easier to read arrays or objects.

## `console.group() / console.groupEnd()`
- **Example:**
  ```javascript
  console.group("Group 1");
  console.log("Message 1");
  console.log("Message 2");
  console.groupEnd();
  ```
- **Explanation:** Groups related log messages together in a collapsible group, making it easier to organize and understand complex logs.

## `console.time() / console.timeEnd()`
- **Example:**
  ```javascript
  console.time("Timer");
  // Code to measure execution time
  console.timeEnd("Timer");
  ```
- **Explanation:** Measures the time it takes to execute a block of code between `console.time()` and `console.timeEnd()` calls, allowing for performance optimization.

## `console.count()`
- **Example:**
  ```javascript
  const fruits = ["apple", "banana", "apple", "orange"];
  fruits.forEach((fruit) => {
    console.count(fruit);
  });
  ```
- **Explanation:** Counts the number of times `console.count()` is called with the same label, useful for tracking the frequency of occurrences.

## `console.trace()`
- **Example:**
  ```javascript
  function foo() {
    bar();
  }
  function bar() {
    console.trace();
  }
  foo();
  ```
- **Explanation:** Outputs a stack trace to the console, showing the function call path that led to the current point of execution. Useful for debugging.

## `console.dir()`
- **Example:**
  ```javascript
  const obj = { a: 1, b: 2 };
  console.dir(obj);
  ```
- **Explanation:** Outputs a JavaScript representation of the specified object to the console. This can be useful for exploring complex objects in more detail.

## `console.profile() / console.profileEnd()`
- **Example:**
  ```javascript
  console.profile("MyProfile");
  // Code to profile
  console.profileEnd("MyProfile");
  ```
- **Explanation:** Initiates and stops the JavaScript profiler under the label provided, allowing developers to analyze the performance profile of a section of code.

## `console.timeStamp()`
- **Example:**
  ```javascript
  console.timeStamp("Event occurred");
  ```
- **Explanation:** Adds a timestamp marker to the browser's timeline, which can be useful for tracking events and performance analysis.

## `console.markTimeline()`
- **Example:**
  ```javascript
  console.markTimeline("Event occurred");
  ```
- **Explanation:** Marks the timeline with the specified label, which can be useful for tracking events and performance analysis.

## `console.timeLog()`
- **Example:**
  ```javascript
  console.time("Timer");
  // Code to measure execution time
  console.timeLog("Timer", "Intermediate log");
  // More code
  console.timeEnd("Timer");
  ```
- **Explanation:** Logs intermediate messages with a timestamp during the execution of a timer set by `console.time()`.

## `console.memory`
- **Example:**
  ```javascript
  console.log(console.memory);
  ```
- **Explanation:** Provides information about the memory usage of the page, including `jsHeapSizeLimit`, `usedJSHeapSize`, and `totalJSHeapSize`.

## `console.global`
- **Example:**
  ```javascript
  console.log(console.global);
  ```
- **Explanation:** Outputs the global object, which is `window` in web browsers and `global` in Node.js environments.

## `console.exception()`
- **Example:**
  ```javascript
  try {
    throw new Error("Custom error");
  } catch (error) {
    console.exception(error);
  }
  ```
- **Explanation:** Logs an exception object to the console, providing detailed information about the error, including the stack trace.

## `console.memory.profile() / console.memory.profileEnd()`
- **Example:**
  ```javascript
  console.memory.profile("MemoryProfile");
  // Code to profile memory usage
  console.memory.profileEnd("MemoryProfile");
  ```
- **Explanation:** Initiates and stops the memory profiler under the label provided, allowing developers to analyze memory usage.

## `console.memory.timeline()`
- **Example:**
  ```javascript
  console.memory.timeline("MemoryEvent");
  ```
- **Explanation:** Marks the timeline with the specified label, capturing memory information at that point, useful for memory profiling.
