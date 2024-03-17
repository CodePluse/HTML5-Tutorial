### 1. `getElementById()`
- **Example**: 
  ```javascript
  const element = document.getElementById("myElement");
  ```
- **Explanation**: Retrieves an element from the DOM with the specified ID.

### 2. `getElementsByClassName()`
- **Example**: 
  ```javascript
  const elements = document.getElementsByClassName("myClass");
  ```
- **Explanation**: Retrieves a collection of elements from the DOM that have the specified class name.

### 3. `getElementsByTagName()`
- **Example**: 
  ```javascript
  const elements = document.getElementsByTagName("div");
  ```
- **Explanation**: Retrieves a collection of elements from the DOM that have the specified tag name.

### 4. `querySelector()`
- **Example**: 
  ```javascript
  const element = document.querySelector("#myElement .myClass");
  ```
- **Explanation**: Returns the first element within the document that matches the specified selector.

### 5. `querySelectorAll()`
- **Example**: 
  ```javascript
  const elements = document.querySelectorAll(".myClass");
  ```
- **Explanation**: Returns a static (non-live) NodeList representing a list of elements that match the specified group of selectors.

### 6. `createElement()`
- **Example**: 
  ```javascript
  const newElement = document.createElement("div");
  ```
- **Explanation**: Creates a new HTML element with the specified tag name.

### 7. `appendChild()`
- **Example**: 
  ```javascript
  parentElement.appendChild(newElement);
  ```
- **Explanation**: Appends a node as the last child of a node.

### 8. `removeChild()`
- **Example**: 
  ```javascript
  parentElement.removeChild(childElement);
  ```
- **Explanation**: Removes a child node from the DOM.

### 9. `setAttribute()`
- **Example**: 
  ```javascript
  element.setAttribute("class", "newClass");
  ```
- **Explanation**: Sets the value of an attribute on the specified element.

### 10. `getAttribute()`
- **Example**: 
  ```javascript
  const value = element.getAttribute("class");
  ```
- **Explanation**: Retrieves the value of the specified attribute on the element.

### 11. `addEventListener()`
- **Example**: 
  ```javascript
  element.addEventListener("click", handleClick);
  ```
- **Explanation**: Adds an event listener to the specified element, invoking a specified function when the event is triggered.

### 12. `removeEventListener()`
- **Example**: 
  ```javascript
  element.removeEventListener("click", handleClick);
  ```
- **Explanation**: Removes an event listener from the specified element.

### 13. `classList`
- **Example**: 
  ```javascript
  element.classList.add("newClass");
  ```
- **Explanation**: Provides methods to add, remove, toggle, and check for the presence of CSS classes on an element.

### 14. `style`
- **Example**: 
  ```javascript
  element.style.color = "red";
  ```
- **Explanation**: Provides access to an element's inline CSS styles, allowing you to manipulate them directly.

### 15. `innerHTML`
- **Example**: 
  ```javascript
  element.innerHTML = "<p>Hello, world!</p>";
  ```
- **Explanation**: Gets or sets the HTML or XML markup contained within the element.

### 16. `innerText`
- **Example**: 
  ```javascript
  element.innerText = "Hello, world!";
  ```
- **Explanation**: Gets or sets the text content of the specified element, and all its descendants.

### 17. `textContent`
- **Example**: 
  ```javascript
  const text = element.textContent;
  ```
- **Explanation**: Gets or sets the text content of the specified element, and all its descendants, preserving whitespace.

### 18. `parentNode`
- **Example**: 
  ```javascript
  const parent = element.parentNode;
  ```
- **Explanation**: Returns the parent node of the specified element.

### 19. `children`
- **Example**: 
  ```javascript
  const childNodes = parentElement.children;
  ```
- **Explanation**: Returns a live HTMLCollection containing all child elements of the specified parent element.

### 20. `querySelector()` (on elements)
- **Example**: 
  ```javascript
  const element = parentElement.querySelector(".myClass");
  ```
- **Explanation**: Returns the first element that is a descendant of the specified parent element and matches the specified selector.

### 21. `querySelectorAll()` (on elements)
- **Example**: 
  ```javascript
  const elements = parentElement.querySelectorAll(".myClass");
  ```
- **Explanation**: Returns a static (non-live) NodeList representing a list of the parent element's descendants that match the specified group of selectors.

### 22. `insertAdjacentHTML()`
- **Example**: 
  ```javascript
  parentElement.insertAdjacentHTML('beforeend', '<p>Hello, world!</p>');
  ```
- **Explanation**: Parses the specified text as HTML or XML and inserts the resulting nodes into the DOM tree at a specified position relative to the element.

### 23. `scrollIntoView()`
- **Example**: 
  ```javascript
  element.scrollIntoView({ behavior: "smooth", block: "end", inline: "nearest" });
  ```
- **Explanation**: Scrolls the element into view within its containing scrollable ancestor, with customizable options such as smooth scrolling and alignment behavior.

### 24. `closest()`
- **Example**: 
  ```javascript
  const closestParent = element.closest('.parentSelector');
  ```
- **Explanation**: Returns the closest ancestor of the current element (or the element itself) that matches the specified group of selectors.

### 25. `contains()`
- **Example**: 
  ```javascript
  const isContained = parentElement.contains(childElement);
  ```
- **Explanation**: Returns a Boolean value indicating whether a node is a descendant of a specified parent node.

### 26. `getAttribute()`
- **Example**: 
  ```javascript
  const value = element.getAttribute("data-id");
  ```
- **Explanation**: Retrieves the value of the specified attribute on the element.

### 27. `setAttribute()`
- **Example**: 
  ```javascript
  element.setAttribute("data-id", "123");
  ```
- **Explanation**: Sets the value of an attribute on the specified element.

### 28. `removeAttribute()`
- **Example**: 
  ```javascript
  element.removeAttribute("data-id");
  ```
- **Explanation**: Removes the specified attribute from the element.

### 29. `getBoundingClientRect()`
- **Example**: 
  ```javascript
  const rect = element.getBoundingClientRect();
  console.log(rect.top, rect.left, rect.width, rect.height);
  ```
- **Explanation**: Returns the size of an element and its position relative to the viewport.

### 30. `scrollTo()`
- **Example**: 
  ```javascript
  window.scrollTo({
    top: 0,
    behavior: 'smooth'
  });
  ```
- **Explanation**: Scrolls the window to a specified position.

### 31. `scrollBy()`
- **Example**: 
  ```javascript
  window.scrollBy({
    top: 100,
    left: 0,
    behavior: 'smooth'
  });
  ```
- **Explanation**: Scrolls the window by a specified number of pixels.

### 32. `requestAnimationFrame()`
- **Example**: 
  ```javascript
  function animate() {
    // Animation logic
    requestAnimationFrame(animate);
  }
  requestAnimationFrame(animate);
  ```
- **Explanation**: Requests that the browser call a specified function to update an animation before the next repaint.

### 33. `cancelAnimationFrame()`
- **Example**: 
  ```javascript
  const animationId = requestAnimationFrame(animate);
  cancelAnimationFrame(animationId);
  ```
- **Explanation**: Cancels a scheduled animation frame request previously scheduled using `requestAnimationFrame()`.

### 34. `createDocumentFragment()`
- **Example**: 
  ```javascript
  const fragment = document.createDocumentFragment();
  ```
- **Explanation**: Creates a new empty DocumentFragment node, which can be used as a lightweight container to store multiple nodes before adding them to the DOM.

### 35. `importNode()`
- **Example**: 
  ```javascript
  const importedNode = document.importNode(template.content, true);
  ```
- **Explanation**: Imports a node from another document or from a template's content document, creating a copy of the node that can be inserted into the current document.

### 36. `focus()`
- **Example**: 
  ```javascript
  inputElement.focus();
  ```
- **Explanation**: Sets focus on the specified element, typically an input element, allowing it to receive keyboard input.

### 37. `blur()`
- **Example**: 
  ```javascript
  inputElement.blur();
  ```
- **Explanation**: Removes focus from the specified element, typically an input element, removing its ability to receive keyboard input.

### 38. `createElementNS()`
- **Example**: 
  ```javascript
  const svgElement = document.createElementNS("http://www.w3.org/2000/svg", "svg");
  ```
- **Explanation**: Creates a new element with the specified namespace URI and qualified name.

### 39. `createTextNode()`
- **Example**: 
  ```javascript
  const textNode = document.createTextNode("Hello, world!");
  ```
- **Explanation**: Creates a new text node with the specified text content.

### 40. `createAttribute()`
- **Example**: 
  ```javascript
  const attribute = document.createAttribute("data-id");
  ```
- **Explanation**: Creates a new attribute node with the specified name.

### 41. `createEvent()`
- **Example**: 
  ```javascript
  const event = document.createEvent("Event");
  event.initEvent("customEvent", true, true);
  ```
- **Explanation**: Creates a new event object of the specified type.

### 42. `dispatchEvent()`
- **Example**: 
  ```javascript
  element.dispatchEvent(event);
  ```
- **Explanation**: Dispatches an event to the specified target, triggering any event listeners that have been registered for the event type.

### 43. `createRange()`
- **Example**: 
  ```javascript
  const range = document.createRange();
  ```
- **Explanation**: Creates a new Range object, which represents a fragment of the document that can contain nodes and parts of text nodes.

### 44. `createComment()`
- **Example**: 
  ```javascript
  const commentNode = document.createComment("This is a comment");
  ```
- **Explanation**: Creates a new comment node with the specified text content.

### 45. `hasChildNodes()`
- **Example**: 
  ```javascript
  const hasChildren = parentElement.hasChildNodes();
  ```
- **Explanation**: Returns a Boolean value indicating whether the specified element has any child nodes.

### 46. `normalize()`
- **Example**: 
  ```javascript
  parentElement.normalize();
  ```
- **Explanation**: Merges adjacent text nodes and removes empty text nodes within the specified element.

### 47. `adoptNode()`
- **Example**: 
  ```javascript
  const adoptedNode = document.adoptNode(externalNode);
  ```
- **Explanation**: Adopts a node from another document or from a template's content document, transferring it to the current document.

### 48. `querySelector()` (on Document)
- **Example**: 
  ```javascript
  const element = document.querySelector(".myClass");
  ```
- **Explanation**: Returns the first element within the document that matches the specified selector.

### 49. `querySelectorAll()` (on Document)
- **Example**: 
  ```javascript
  const elements = document.querySelectorAll(".myClass");
  ```
- **Explanation**: Returns a static (non-live) NodeList representing a list of elements within the document that match the specified group of selectors.

### 50. `createElement()`
- **Example**: 
  ```javascript
  const newElement = document.createElement("div");
  ```
- **Explanation**: Creates a new HTML element with the specified tag name.

### 51. `createTextNode()`
- **Example**: 
  ```javascript
  const textNode = document.createTextNode("Hello, world!");
  ```
- **Explanation**: Creates a new text node with the specified text content.

### 52. `createDocumentFragment()`
- **Example**: 
  ```javascript
  const fragment = document.createDocumentFragment();
  ```
- **Explanation**: Creates a new empty DocumentFragment node, which can be used as a lightweight container to store multiple nodes before adding them to the DOM.

### 53. `importNode()`
- **Example**: 
  ```javascript
  const importedNode = document.importNode(template.content, true);
  ```
- **Explanation**: Imports a node from another document or from a template's content document, creating a copy of the node that can be inserted into the current document.

### 54. `addEventListener()`
- **Example**: 
  ```javascript
  document.addEventListener("DOMContentLoaded", () => {
    // Code to run when the document has finished loading
  });
  ```
- **Explanation**: Adds an event listener to the document, which listens for a specific event type and invokes a specified function when the event is triggered.

### 55. `removeEventListener()`
- **Example**: 
  ```javascript
  const handleClick = () => {
    // Code to handle click event
  };
  document.removeEventListener("click", handleClick);
  ```
- **Explanation**: Removes an event listener from the document.

### 56. `getElementById()`
- **Example**: 
  ```javascript
  const element = document.getElementById("myElement");
  ```
- **Explanation**: Retrieves an element from the document with the specified ID.

### 57. `getElementsByClassName()`
- **Example**: 
  ```javascript
  const elements = document.getElementsByClassName("myClass");
  ```
- **Explanation**: Retrieves a collection of elements from the document that have the specified class name.

### 58. `getElementsByTagName()`
- **Example**: 
  ```javascript
  const elements = document.getElementsByTagName("div");
  ```
- **Explanation**: Retrieves a collection of elements from the document that have the specified tag name.

### 59. `getElementsByName()`
- **Example**: 
  ```javascript
  const elements = document.getElementsByName("myName");
  ```
- **Explanation**: Retrieves a collection of elements from the document that have the specified name attribute value.

### 60. `querySelector()` (on elements)
- **Example**: 
  ```javascript
  const element = parentElement.querySelector(".myClass");
  ```
- **Explanation**: Returns the first element that is a descendant of the specified parent element and matches the specified selector.

### 61. `querySelectorAll()` (on elements)
- **Example**: 
  ```javascript
  const elements = parentElement.querySelectorAll(".myClass");
  ```
- **Explanation**: Returns a static (non-live) NodeList representing a list of the parent element's descendants that match the specified group of selectors.

### 62. `appendChild()`
- **Example**: 
  ```javascript
  parentElement.appendChild(newElement);
  ```
- **Explanation**: Appends a node as the last child of a node.

### 63. `removeChild()`
- **Example**: 
  ```javascript
  parentElement.removeChild(childElement);
  ```
- **Explanation**: Removes a child node from the parent element.

### 64. `insertBefore()`
- **Example**: 
  ```javascript
  parentElement.insertBefore(newElement, referenceElement);
  ```
- **Explanation**: Inserts a node before a specified reference node as a child of the parent element.

### 65. `replaceChild()`
- **Example**: 
  ```javascript
  parentElement.replaceChild(newElement, oldElement);
  ```
- **Explanation**: Replaces a child node of the parent element with a new node.

### 66. `cloneNode()`
- **Example**: 
  ```javascript
  const clonedNode = originalNode.cloneNode(true);
  ```
- **Explanation**: Creates a copy of the specified node, optionally including its descendants.

### 67. `addEventListener()`
- **Example**: 
  ```javascript
  element.addEventListener("click", handleClick);
  ```
- **Explanation**: Adds an event listener to the specified element, which listens for a specific event type and invokes a specified function when the event is triggered.

### 68. `removeEventListener()`
- **Example**: 
  ```javascript
  element.removeEventListener("click", handleClick);
  ```
- **Explanation**: Removes an event listener from the specified element.

### 69. `classList`
- **Example**: 
  ```javascript
  element.classList.add("newClass");
  ```
- **Explanation**: Provides methods to add, remove, toggle, and check for the presence of CSS classes on an element.

### 70. `style`
- **Example**: 
  ```javascript
  element.style.color = "red";
  ```
- **Explanation**: Provides access to an element's inline CSS styles, allowing you to manipulate them directly.

### 71. `setAttribute()`
- **Example**: 
  ```javascript
  element.setAttribute("data-id", "123");
  ```
- **Explanation**: Sets the value of an attribute on the specified element.

### 72. `getAttribute()`
- **Example**: 
  ```javascript
  const value = element.getAttribute("data-id");
  ```
- **Explanation**: Retrieves the value of the specified attribute on the element.

### 73. `removeAttribute()`
- **Example**: 
  ```javascript
  element.removeAttribute("data-id");
  ```
- **Explanation**: Removes the specified attribute from the element.

### 74. `innerHTML`
- **Example**: 
  ```javascript
  element.innerHTML = "<p>Hello, world!</p>";
  ```
- **Explanation**: Gets or sets the HTML or XML markup contained within the element.

### 75. `innerText`
- **Example**: 
  ```javascript
  element.innerText = "Hello, world!";
  ```
- **Explanation**: Gets or sets the text content of the element, including its descendants, with HTML markup escaped.

### 76. `textContent`
- **Example**: 
  ```javascript
  const text = element.textContent;
  ```
- **Explanation**: Gets or sets the text content of the element, including its descendants, with whitespace and HTML markup preserved.

### 77. `scrollIntoView()`
- **Example**: 
  ```javascript
  element.scrollIntoView({ behavior: "smooth", block: "end", inline: "nearest" });
  ```
- **Explanation**: Scrolls the element into view within its containing scrollable ancestor, with customizable options such as smooth scrolling and alignment behavior.

### 78. `getBoundingClientRect()`
- **Example**: 
  ```javascript
  const rect = element.getBoundingClientRect();
  console.log(rect.top, rect.left, rect.width, rect.height);
  ```
- **Explanation**: Returns the size of an element and its position relative to the viewport.

### 79. `setAttribute()`
- **Example**: 
  ```javascript
  element.setAttribute("class", "newClass");
  ```
- **Explanation**: Sets the value of an attribute on the specified element.

### 80. `getAttribute()`
- **Example**: 
  ```javascript
  const value = element.getAttribute("class");
  ```
- **Explanation**: Retrieves the value of the specified attribute on the element.

### 81. `removeAttribute()`
- **Example**: 
  ```javascript
  element.removeAttribute("class");
  ```
- **Explanation**: Removes the specified attribute from the element.

### 82. `hasAttribute()`
- **Example**: 
  ```javascript
  const hasClass = element.hasAttribute("class");
  ```
- **Explanation**: Returns a Boolean value indicating whether the element has the specified attribute.

### 83. `matches()`
- **Example**: 
  ```javascript
  const isMatch = element.matches(".myClass");
  ```
- **Explanation**: Returns a Boolean value indicating whether the element matches the specified CSS selector.

### 84. `closest()`
- **Example**: 
  ```javascript
  const closestParent = element.closest('.parentSelector');
  ```
- **Explanation**: Returns the closest ancestor of the current element (or the element itself) that matches the specified group of selectors.

### 85. `contains()`
- **Example**: 
  ```javascript
  const isContained = parentElement.contains(childElement);
  ```
- **Explanation**: Returns a Boolean value indicating whether a node is a descendant of a specified parent node.

### 86. `focus()`
- **Example**: 
  ```javascript
  inputElement.focus();
  ```
- **Explanation**: Sets focus on the specified element, typically an input element, allowing it to receive keyboard input.

### 87. `blur()`
- **Example**: 
  ```javascript
  inputElement.blur();
  ```
- **Explanation**: Removes focus from the specified element, typically an input element, removing its ability to receive keyboard input.

### 88. `scrollTo()`
- **Example**: 
  ```javascript
  window.scrollTo({
    top: 0,
    left: 0,
    behavior: 'smooth'
  });
  ```
- **Explanation**: Scrolls the window to a specified position, with options for smooth scrolling behavior.

### 89. `scrollBy()`
- **Example**: 
  ```javascript
  window.scrollBy({
    top: 100,
    left: 0,
    behavior: 'smooth'
  });
  ```
- **Explanation**: Scrolls the window by a specified number of pixels, with options for smooth scrolling behavior.

### 90. `scrollIntoView()`
- **Example**: 
  ```javascript
  element.scrollIntoView({ behavior: "smooth", block: "end", inline: "nearest" });
  ```
- **Explanation**: Scrolls the element into view within its containing scrollable ancestor, with customizable options such as smooth scrolling and alignment behavior.

### 91. `requestAnimationFrame()`
- **Example**: 
  ```javascript
  function animate() {
    // Animation logic
    requestAnimationFrame(animate);
  }
  requestAnimationFrame(animate);
  ```
- **Explanation**: Requests that the browser call a specified function to update an animation before the next repaint.

### 92. `cancelAnimationFrame()`
- **Example**: 
  ```javascript
  const animationId = requestAnimationFrame(animate);
  cancelAnimationFrame(animationId);
  ```
- **Explanation**: Cancels a scheduled animation frame request previously scheduled using `requestAnimationFrame()`.

### 93. `createElementNS()`
- **Example**: 
  ```javascript
  const svgElement = document.createElementNS("http://www.w3.org/2000/svg", "svg");
  ```
- **Explanation**: Creates a new element with the specified namespace URI and qualified name.

### 94. `createAttribute()`
- **Example**: 
  ```javascript
  const attribute = document.createAttribute("data-id");
  ```
- **Explanation**: Creates a new attribute node with the specified name.

### 95. `createEvent()`
- **Example**: 
  ```javascript
  const event = document.createEvent("Event");
  event.initEvent("customEvent", true, true);
  ```
- **Explanation**: Creates a new event object of the specified type.

### 96. `dispatchEvent()`
- **Example**: 
  ```javascript
  element.dispatchEvent(event);
  ```
- **Explanation**: Dispatches an event to the specified target, triggering any event listeners that have been registered for the event type.

### 97. `createRange()`
- **Example**: 
  ```javascript
  const range = document.createRange();
  ```
- **Explanation**: Creates a new Range object, which represents a fragment of the document that can contain nodes and parts of text nodes.

### 98. `createComment()`
- **Example**: 
  ```javascript
  const commentNode = document.createComment("This is a comment");
  ```
- **Explanation**: Creates a new comment node with the specified text content.

### 99. `createProcessingInstruction()`
- **Example**: 
  ```javascript
  const piNode = document.createProcessingInstruction("xml-stylesheet", "href=\"style.css\"");
  ```
- **Explanation**: Creates a new processing instruction node with the specified target and data.

### 100. `hasFocus()`
- **Example**: 
  ```javascript
  const hasFocus = element.hasFocus();
  ```
- **Explanation**: Returns a Boolean value indicating whether the element has focus.

### 101. `createCDATASection()`
- **Example**: 
  ```javascript
  const cdataNode = document.createCDATASection("<![CDATA[This is CDATA content]]>");
  ```
- **Explanation**: Creates a new CDATASection node with the specified data.

### 102. `createEntityReference()`
- **Example**: 
  ```javascript
  const entityRefNode = document.createEntityReference("entityName");
  ```
- **Explanation**: Creates a new EntityReference node with the specified entity name.

### 103. `createProcessingInstruction()`
- **Example**: 
  ```javascript
  const piNode = document.createProcessingInstruction("xml-stylesheet", "href=\"style.css\"");
  ```
- **Explanation**: Creates a new processing instruction node with the specified target and data.

### 104. `createTextNode()`
- **Example**: 
  ```javascript
  const textNode = document.createTextNode("Hello, world!");
  ```
- **Explanation**: Creates a new text node with the specified text content.

### 105. `createRange()`
- **Example**: 
  ```javascript
  const range = document.createRange();
  ```
- **Explanation**: Creates a new Range object, which represents a fragment of the document that can contain nodes and parts of text nodes.

### 106. `createTreeWalker()`
- **Example**: 
  ```javascript
  const treeWalker = document.createTreeWalker(rootNode, NodeFilter.SHOW_ELEMENT, { acceptNode: node => NodeFilter.FILTER_ACCEPT });
  ```
- **Explanation**: Creates a new TreeWalker object, which can be used to traverse the nodes of a document subtree and perform custom filtering and processing.

### 107. `getElementsByClassName()`
- **Example**: 
  ```javascript
  const elements = document.getElementsByClassName("myClass");
  ```
- **Explanation**: Retrieves a collection of elements from the document that have the specified class name.

### 108. `getElementsByTagName()`
- **Example**: 
  ```javascript
  const elements = document.getElementsByTagName("div");
  ```
- **Explanation**: Retrieves a collection of elements from the document that have the specified tag name.

### 109. `getElementsByName()`
- **Example**: 
  ```javascript
  const elements = document.getElementsByName("myName");
  ```
- **Explanation**: Retrieves a collection of elements from the document that have the specified name attribute value.

### 110. `hasFocus()`
- **Example**: 
  ```javascript
  const hasFocus = element.hasFocus();
  ```
- **Explanation**: Returns a Boolean value indicating whether the element has focus.

### 111. `querySelector()`
- **Example**: 
  ```javascript
  const element = document.querySelector(".myClass");
  ```
- **Explanation**: Returns the first element within the document that matches the specified selector.

### 112. `querySelectorAll()`
- **Example**: 
  ```javascript
  const elements = document.querySelectorAll(".myClass");
  ```
- **Explanation**: Returns a static (non-live) NodeList representing a list of elements within the document that match the specified group of selectors.

### 113. `write()`
- **Example**: 
  ```javascript
  document.write("Hello, world!");
  ```
- **Explanation**: Writes HTML content to the document stream, replacing any existing content.

### 114. `writeln()`
- **Example**: 
  ```javascript
  document.writeln("Hello, world!");
  ```
- **Explanation**: Writes HTML content followed by a newline character to the document stream, replacing any existing content.

### 115. `querySelector()` (on elements)
- **Example**: 
  ```javascript
  const element = parentElement.querySelector(".myClass");
  ```
- **Explanation**: Returns the first element that is a descendant of the specified parent element and matches the specified selector.

### 116. `querySelectorAll()` (on elements)
- **Example**: 
  ```javascript
  const elements = parentElement.querySelectorAll(".myClass");
  ```
- **Explanation**: Returns a static (non-live) NodeList representing a list of the parent element's descendants that match the specified group of selectors.

### 117. `appendChild()`
- **Example**: 
  ```javascript
  parentElement.appendChild(newElement);
  ```
- **Explanation**: Appends a node as the last child of a node.

### 118. `removeChild()`
- **Example**: 
  ```javascript
  parentElement.removeChild(childElement);
  ```
- **Explanation**: Removes a child node from the parent element.

### 119. `insertBefore()`
- **Example**: 
  ```javascript
  parentElement.insertBefore(newElement, referenceElement);
  ```
- **Explanation**: Inserts a node before a specified reference node as a child of the parent element.

### 120. `replaceChild()`
- **Example**: 
  ```javascript
  parentElement.replaceChild(newElement, oldElement);
  ```
- **Explanation**: Replaces a child node of the parent element with a new node.

### 121. `cloneNode()`
- **Example**: 
  ```javascript
  const clonedNode = originalNode.cloneNode(true);
  ```
- **Explanation**: Creates a copy of the specified node, optionally including its descendants.

### 122. `addEventListener()`
- **Example**: 
  ```javascript
  element.addEventListener("click", handleClick);
  ```
- **Explanation**: Adds an event listener to the specified element, which listens for a specific event type and invokes a specified function when the event is triggered.

### 123. `removeEventListener()`
- **Example**: 
  ```javascript
  element.removeEventListener("click", handleClick);
  ```
- **Explanation**: Removes an event listener from the specified element.

### 124. `classList`
- **Example**: 
  ```javascript
  element.classList.add("newClass");
  ```
- **Explanation**: Provides methods to add, remove, toggle, and check for the presence of CSS classes on an element.

### 125. `style`
- **Example**: 
  ```javascript
  element.style.color = "red";
  ```
- **Explanation**: Provides access to an element's inline CSS styles, allowing you to manipulate them directly.

### 126. `setAttribute()`
- **Example**: 
  ```javascript
  element.setAttribute("data-id", "123");
  ```
- **Explanation**: Sets the value of an attribute on the specified element.

### 127. `getAttribute()`
- **Example**: 
  ```javascript
  const value = element.getAttribute("data-id");
  ```
- **Explanation**: Retrieves the value of the specified attribute on the element.

### 128. `removeAttribute()`
- **Example**: 
  ```javascript
  element.removeAttribute("data-id");
  ```
- **Explanation**: Removes the specified attribute from the element.

### 129. `hasAttribute()`
- **Example**: 
  ```javascript
  const hasClass = element.hasAttribute("class");
  ```
- **Explanation**: Returns a Boolean value indicating whether the element has the specified attribute.

### 130. `matches()`
- **Example**: 
  ```javascript
  const isMatch = element.matches(".myClass");
  ```
- **Explanation**: Returns a Boolean value indicating whether the element matches the specified CSS selector.

### 131. `closest()`
- **Example**: 
  ```javascript
  const closestParent = element.closest('.parentSelector');
  ```
- **Explanation**: Returns the closest ancestor of the current element (or the element itself) that matches the specified group of selectors.

### 132. `contains()`
- **Example**: 
  ```javascript
  const isContained = parentElement.contains(childElement);
  ```
- **Explanation**: Returns a Boolean value indicating whether a node is a descendant of a specified parent node.

### 133. `focus()`
- **Example**: 
  ```javascript
  inputElement.focus();
  ```
- **Explanation**: Sets focus on the specified element, typically an input element, allowing it to receive keyboard input.

### 134. `blur()`
- **Example**: 
  ```javascript
  inputElement.blur();
  ```
- **Explanation**: Removes focus from the specified element, typically an input element, removing its ability to receive keyboard input.

### 135. `scrollTo()`
- **Example**: 
  ```javascript
  window.scrollTo({
    top: 0,
    left: 0,
    behavior: 'smooth'
  });
  ```
- **Explanation**: Scrolls the window to a specified position, with options for smooth scrolling behavior.

### 136. `scrollBy()`
- **Example**: 
  ```javascript
  window.scrollBy({
    top: 100,
    left: 0,
    behavior: 'smooth'
  });
  ```
- **Explanation**: Scrolls the window by a specified number of pixels, with options for smooth scrolling behavior.

### 137. `scrollIntoView()`
- **Example**: 
  ```javascript
  element.scrollIntoView({ behavior: "smooth", block: "end", inline: "nearest" });
  ```
- **Explanation**: Scrolls the element into view within its containing scrollable ancestor, with customizable options such as smooth scrolling and alignment behavior.

### 138. `requestAnimationFrame()`
- **Example**: 
  ```javascript
  function animate() {
    // Animation logic
    requestAnimationFrame(animate);
  }
  requestAnimationFrame(animate);
  ```
- **Explanation**: Requests that the browser call a specified function to update an animation before the next repaint.

### 139. `cancelAnimationFrame()`
- **Example**: 
  ```javascript
  const animationId = requestAnimationFrame(animate);
  cancelAnimationFrame(animationId);
  ```
- **Explanation**: Cancels a scheduled animation frame request previously scheduled using `requestAnimationFrame()`.

### 140. `createDocumentFragment()`
- **Example**: 
  ```javascript
  const fragment = document.createDocumentFragment();
  ```
- **Explanation**: Creates a new empty DocumentFragment node, which can be used as a lightweight container to store multiple nodes before adding them to the DOM.

### 141. `importNode()`
- **Example**: 
  ```javascript
  const importedNode = document.importNode(template.content, true);
  ```
- **Explanation**: Imports a node from another document or from a template's content document, creating a copy of the node that can be inserted into the current document.

### 142. `createElement()`
- **Example**: 
  ```javascript
  const newElement = document.createElement("div");
  ```
- **Explanation**: Creates a new HTML element with the specified tag name.

### 143. `createAttribute()`
- **Example**: 
  ```javascript
  const attribute = document.createAttribute("data-id");
  ```
- **Explanation**: Creates a new attribute node with the specified name.

### 144. `createEvent()`
- **Example**: 
  ```javascript
  const event = document.createEvent("Event");
  event.initEvent("customEvent", true, true);
  ```
- **Explanation**: Creates a new event object of the specified type.

### 145. `dispatchEvent()`
- **Example**: 
  ```javascript
  element.dispatchEvent(event);
  ```
- **Explanation**: Dispatches an event to the specified target, triggering any event listeners that have been registered for the event type.

### 146. `createCDATASection()`
- **Example**: 
  ```javascript
  const cdataNode = document.createCDATASection("<![CDATA[This is CDATA content]]>");
  ```
- **Explanation**: Creates a new CDATASection node with the specified data.

### 147. `createEntityReference()`
- **Example**: 
  ```javascript
  const entityRefNode = document.createEntityReference("entityName");
  ```
- **Explanation**: Creates a new EntityReference node with the specified entity name.

### 148. `createProcessingInstruction()`
- **Example**: 
  ```javascript
  const piNode = document.createProcessingInstruction("xml-stylesheet", "href=\"style.css\"");
  ```
- **Explanation**: Creates a new processing instruction node with the specified target and data.

### 149. `createTextNode()`
- **Example**: 
  ```javascript
  const textNode = document.createTextNode("Hello, world!");
  ```
- **Explanation**: Creates a new text node with the specified text content.

### 150. `createRange()`
- **Example**: 
  ```javascript
  const range = document.createRange();
  ```
- **Explanation**: Creates a new Range object, which represents a fragment of the document that can contain nodes and parts of text nodes.

### 151. `createTreeWalker()`
- **Example**: 
  ```javascript
  const treeWalker = document.createTreeWalker(rootNode, NodeFilter.SHOW_ELEMENT, { acceptNode: node => NodeFilter.FILTER_ACCEPT });
  ```
- **Explanation**: Creates a new TreeWalker object, which can be used to traverse the nodes of a document subtree and perform custom filtering and processing.

### 152. `getElementsByClassName()`
- **Example**: 
  ```javascript
  const elements = document.getElementsByClassName("myClass");
  ```
- **Explanation**: Retrieves a collection of elements from the document that have the specified class name.

### 153. `getElementsByTagName()`
- **Example**: 
  ```javascript
  const elements = document.getElementsByTagName("div");
  ```
- **Explanation**: Retrieves a collection of elements from the document that have the specified tag name.

### 154. `getElementsByName()`
- **Example**: 
  ```javascript
  const elements = document.getElementsByName("myName");
  ```
- **Explanation**: Retrieves a collection of elements from the document that have the specified name attribute value.

### 155. `hasFocus()`
- **Example**: 
  ```javascript
  const hasFocus = element.hasFocus();
  ```
- **Explanation**: Returns a Boolean value indicating whether the element has focus.

### 156. `querySelector()`
- **Example**: 
  ```javascript
  const element = document.querySelector(".myClass");
  ```
- **Explanation**: Returns the first element within the document that matches the specified selector.

### 157. `querySelectorAll()`
- **Example**: 
  ```javascript
  const elements = document.querySelectorAll(".myClass");
  ```
- **Explanation**: Returns a static (non-live) NodeList representing a list of elements within the document that match the specified group of selectors.

### 158. `write()`
- **Example**: 
  ```javascript
  document.write("Hello, world!");
  ```
- **Explanation**: Writes HTML content to the document stream, replacing any existing content.

### 159. `writeln()`
- **Example**: 
  ```javascript
  document.writeln("Hello, world!");
  ```
- **Explanation**: Writes HTML content followed by a newline character to the document stream, replacing any existing content.

### 160. `createDocumentFragment()`
- **Example**: 
  ```javascript
  const fragment = document.createDocumentFragment();
  ```
- **Explanation**: Creates a new empty DocumentFragment node, which can be used as a lightweight container to store multiple nodes before adding them to the DOM.

### 161. `importNode()`
- **Example**: 
  ```javascript
  const importedNode = document.importNode(template.content, true);
  ```
- **Explanation**: Imports a node from another document or from a template's content document, creating a copy of the node that can be inserted into the current document.

### 162. `createElement()`
- **Example**: 
  ```javascript
  const newElement = document.createElement("div");
  ```
- **Explanation**: Creates a new HTML element with the specified tag name.

### 163. `createAttribute()`
- **Example**: 
  ```javascript
  const attribute = document.createAttribute("data-id");
  ```
- **Explanation**: Creates a new attribute node with the specified name.

### 164. `createEvent()`
- **Example**: 
  ```javascript
  const event = document.createEvent("Event");
  event.initEvent("customEvent", true, true);
  ```
- **Explanation**: Creates a new event object of the specified type.

### 165. `dispatchEvent()`
- **Example**: 
  ```javascript
  element.dispatchEvent(event);
  ```
- **Explanation**: Dispatches an event to the specified target, triggering any event listeners that have been registered for the event type.

### 166. `createRange()`
- **Example**: 
  ```javascript
  const range = document.createRange();
  ```
- **Explanation**: Creates a new Range object, which represents a fragment of the document that can contain nodes and parts of text nodes.

### 167. `createComment()`
- **Example**: 
  ```javascript
  const commentNode = document.createComment("This is a comment");
  ```
- **Explanation**: Creates a new comment node with the specified text content.

### 168. `createProcessingInstruction()`
- **Example**: 
  ```javascript
  const piNode = document.createProcessingInstruction("xml-stylesheet", "href=\"style.css\"");
  ```
- **Explanation**: Creates a new processing instruction node with the specified target and data.

These methods provide various ways to interact with and manipulate the Document Object Model (DOM) in JavaScript, allowing you to create, query, and traverse elements within the document. Understanding and utilizing these methods effectively is crucial for building dynamic and interactive web applications.
