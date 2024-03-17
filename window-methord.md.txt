# Essential JavaScript Window Methods for Professional Developers

## `window.alert()`
- **Example:**
  ```javascript
  window.alert("Hello, world!");
  ```
- **Explanation:** Displays a dialog box with the specified message and an OK button, pausing script execution until the user dismisses the dialog.

## `window.confirm()`
- **Example:**
  ```javascript
  const result = window.confirm("Are you sure?");
  if (result) {
    console.log("User clicked OK.");
  } else {
    console.log("User clicked Cancel.");
  }
  ```
- **Explanation:** Displays a dialog box with a message and OK/Cancel buttons. Returns `true` if the user clicks OK and `false` if the user clicks Cancel.

## `window.prompt()`
- **Example:**
  ```javascript
  const name = window.prompt("Please enter your name:");
  console.log("Hello, " + name + "!");
  ```
- **Explanation:** Displays a dialog box with a message, an input field, and OK/Cancel buttons. Returns the text entered by the user or `null` if the user clicks Cancel.

## `window.open()`
- **Example:**
  ```javascript
  const newWindow = window.open("https://example.com", "_blank", "width=600,height=400");
  ```
- **Explanation:** Opens a new browser window with the specified URL and options. Returns a reference to the new window object.

## `window.close()`
- **Example:**
  ```javascript
  setTimeout(function() {
    window.close();
  }, 5000);
  ```
- **Explanation:** Closes the current window if it was opened by a script. Note: Modern browsers usually restrict the use of this method for security reasons.

## `window.location`
- **Example:**
  ```javascript
  console.log(window.location.href);
  ```
- **Explanation:** Provides information about the current URL and allows navigation to different URLs. Properties include `href`, `host`, `pathname`, `search`, and more.

## `window.history`
- **Example:**
  ```javascript
  window.history.back();
  ```
- **Explanation:** Provides access to the browser's session history. Methods include `back()`, `forward()`, `go()`, and properties like `length`.

## `window.localStorage` / `window.sessionStorage`
- **Example:**
  ```javascript
  window.localStorage.setItem("username", "John");
  const username = window.localStorage.getItem("username");
  ```
- **Explanation:** Allows storing key-value pairs persistently (`localStorage`) or for the duration of the page session (`sessionStorage`) in the browser.

## `window.setTimeout()` / `window.setInterval()`
- **Example:**
  ```javascript
  const timeoutId = window.setTimeout(function() {
    console.log("Timeout occurred.");
  }, 3000);
  const intervalId = window.setInterval(function() {
    console.log("Interval occurred.");
  }, 2000);
  ```
- **Explanation:** Executes a function or evaluates an expression after a specified delay (`setTimeout`) or repeatedly at specified intervals (`setInterval`).

## `window.clearTimeout()` / `window.clearInterval()`
- **Example:**
  ```javascript
  window.clearTimeout(timeoutId);
  window.clearInterval(intervalId);
  ```
- **Explanation:** Cancels a timeout or interval set by `setTimeout` or `setInterval` respectively.

## `window.scrollTo()`
- **Example:**
  ```javascript
  window.scrollTo({
    top: 0,
    left: 0,
    behavior: 'smooth'
  });
  ```
- **Explanation:** Scrolls the window to the specified coordinates, optionally with smooth animation.

## `window.scrollBy()`
- **Example:**
  ```javascript
  window.scrollBy({
    top: 100,
    left: 0,
    behavior: 'smooth'
  });
  ```
- **Explanation:** Scrolls the window by the specified amount, optionally with smooth animation.

## `window.innerHeight` / `window.innerWidth`
- **Example:**
  ```javascript
  console.log("Window height:", window.innerHeight);
  console.log("Window width:", window.innerWidth);
  ```
- **Explanation:** Returns the height and width of the window's content area (viewport) in pixels.

## `window.outerHeight` / `window.outerWidth`
- **Example:**
  ```javascript
  console.log("Window outer height:", window.outerHeight);
  console.log("Window outer width:", window.outerWidth);
  ```
- **Explanation:** Returns the height and width of the entire browser window including toolbars and scrollbars, in pixels.

## `window.focus()` / `window.blur()`
- **Example:**
  ```javascript
  window.focus();
  ```
- **Explanation:** Brings the window to the front and gives it focus. `window.blur()` removes focus from the window.

## `window.requestAnimationFrame()`
- **Example:**
  ```javascript
  function animate() {
    // Animation logic
    window.requestAnimationFrame(animate);
  }
  animate();
  ```
- **Explanation:** Requests the browser to call a specified function to update an animation before the next repaint. Optimized for smoother animations.

## `window.cancelAnimationFrame()`
- **Example:**
  ```javascript
  const animationId = window.requestAnimationFrame(animate);
  window.cancelAnimationFrame(animationId);
  ```
- **Explanation:** Cancels a previously scheduled animation frame request.

## `window.matchMedia()`
- **Example:**
  ```javascript
  const mediaQuery = window.matchMedia('(max-width: 600px)');
  if (mediaQuery.matches) {
    console.log("Window is less than 600px wide.");
  }
  ```
- **Explanation:** Returns a MediaQueryList object representing the results of the specified CSS media query string.

## `window.getSelection()`
- **Example:**
  ```javascript
  const selection = window.getSelection();
  console.log("Selected text:", selection.toString());
  ```
- **Explanation:** Returns a Selection object representing the currently selected text in the document.

## `window.print()`
- **Example:**
  ```javascript
  window.print();
  ```
- **Explanation:** Opens the browser's print dialog to print the current page.

## `window.getComputedStyle()`
- **Example:**
  ```javascript
  const element = document.getElementById("example");
  const styles = window.getComputedStyle(element);
  console.log("Computed styles:", styles);
  ```
- **Explanation:** Returns the computed styles of an element, including styles applied through CSS and styles inherited from parent elements.

## `window.requestIdleCallback()`
- **Example:**
  ```javascript
  window.requestIdleCallback(function(deadline) {
    console.log("Idle callback executed.");
  });
  ```
- **Explanation:** Requests a callback to be executed during browser idle periods, allowing tasks to be performed without impacting user experience.

## `window.cancelIdleCallback()`
- **Example:**
  ```javascript
  const idleCallbackId = window.requestIdleCallback(myCallback);
  window.cancelIdleCallback(idleCallbackId);
  ```
- **Explanation:** Cancels a previously scheduled idle callback.

## `window.postMessage()`
- **Example:**
  ```javascript
  window.postMessage("Hello from child window!", "https://parentdomain.com");
  ```
- **Explanation:** Sends a message to another window or frame, even if it's on a different origin.

## `window.addEventListener()`
- **Example:**
  ```javascript
  window.addEventListener("resize", function() {
    console.log("Window resized.");
  });
  ```
- **Explanation:** Registers an event listener on the window object to listen for events like resize, scroll, load, etc.

## `window.removeEventListener()`
- **Example:**
  ```javascript
  function resizeHandler() {
    console.log("Window resized.");
  }
  window.addEventListener("resize", resizeHandler);
  window.removeEventListener("resize", resizeHandler);
  ```
- **Explanation:** Removes an event listener previously added with `addEventListener()`.

## `window.crypto.getRandomValues()`
- **Example:**
  ```javascript
  const array = new Uint32Array(1);
  window.crypto.getRandomValues(array);
  console.log("Random value:", array[0]);
  ```
- **Explanation:** Fills the specified typed array with cryptographically random values.

## `window.crypto.subtle.digest()`
- **Example:**
  ```javascript
  const data = new Uint8Array([0, 1, 2, 3]);
  window.crypto.subtle.digest("SHA-256", data).then(hash => {
    console.log("Hash:", hash);
  });
  ```
- **Explanation:** Computes the hash of the given data using the specified algorithm (e.g., SHA-256) in a cryptographically secure manner.

## `window.requestFullscreen()` / `window.exitFullscreen()`
- **Example:**
  ```javascript
  const element = document.getElementById("video");
  element.requestFullscreen();
  // To exit fullscreen:
  // window.exitFullscreen();
  ```
- **Explanation:** Requests entering or exiting fullscreen mode for the document or a specific element.

## `window.navigator`
- **Example:**
  ```javascript
  console.log("User agent:", window.navigator.userAgent);
  ```
- **Explanation:** Provides information about the browser and system environment, including user agent, platform, language, etc.

## `window.matchMedia()`
- **Example:**
  ```javascript
  const mediaQuery = window.matchMedia('(max-width: 600px)');
  if (mediaQuery.matches) {
    console.log("Window is less than 600px wide.");
  }
  ```
- **Explanation:** Returns a MediaQueryList object representing the results of the specified CSS media query string.

## `window.getSelection()`
- **Example:**
  ```javascript
  const selection = window.getSelection();
  console.log("Selected text:", selection.toString());
  ```
- **Explanation:** Returns a Selection object representing the currently selected text in the document.

## `window.print()`
- **Example:**
  ```javascript
  window.print();
  ```
- **Explanation:** Opens the browser's print dialog to print the current page.

## `window.getComputedStyle()`
- **Example:**
  ```javascript
  const element = document.getElementById("example");
  const styles = window.getComputedStyle(element);
  console.log("Computed styles:", styles);
  ```
- **Explanation:** Returns the computed styles of an element, including styles applied through CSS and styles inherited from parent elements.

## `window.requestIdleCallback()`
- **Example:**
  ```javascript
  window.requestIdleCallback(function(deadline) {
    console.log("Idle callback executed.");
  });
  ```
- **Explanation:** Requests a callback to be executed during browser idle periods, allowing tasks to be performed without impacting user experience.

## `window.cancelIdleCallback()`
- **Example:**
  ```javascript
  const idleCallbackId = window.requestIdleCallback(myCallback);
  window.cancelIdleCallback(idleCallbackId);
  ```
- **Explanation:** Cancels a previously scheduled idle callback.

## `window.postMessage()`
- **Example:**
  ```javascript
  window.postMessage("Hello from child window!", "https://parentdomain.com");
  ```
- **Explanation:** Sends a message to another window or frame, even if it's on a different origin.

## `window.addEventListener()`
- **Example:**
  ```javascript
  window.addEventListener("resize", function() {
    console.log("Window resized.");
  });
  ```
- **Explanation:** Registers an event listener on the window object to listen for events like resize, scroll, load, etc.

## `window.removeEventListener()`
- **Example:**
  ```javascript
  function resizeHandler() {
    console.log("Window resized.");
  }
  window.addEventListener("resize", resizeHandler);
  window.removeEventListener("resize", resizeHandler);
  ```
- **Explanation:** Removes an event listener previously added with `addEventListener()`.

## `window.crypto.getRandomValues()`
- **Example:**
  ```javascript
  const array = new Uint32Array(1);
  window.crypto.getRandomValues(array);
  console.log("Random value:", array[0]);
  ```
- **Explanation:** Fills the specified typed array with cryptographically random values.

## `window.crypto.subtle.digest()`
- **Example:**
  ```javascript
  const data = new Uint8Array([0, 1, 2, 3]);
  window.crypto.subtle.digest("SHA-256", data).then(hash => {
    console.log("Hash:", hash);
  });
  ```
- **Explanation:** Computes the hash of the given data using the specified algorithm (e.g., SHA-256) in a cryptographically secure manner.

## `window.requestFullscreen()` / `window.exitFullscreen()`
- **Example:**
  ```javascript
  const element = document.getElementById("video");
  element.requestFullscreen();
  // To exit fullscreen:
  // window.exitFullscreen();
  ```
- **Explanation:** Requests entering or exiting fullscreen mode for the document or a specific element.

## `window.navigator`
- **Example:**
  ```javascript
  console.log("User agent:", window.navigator.userAgent);
  ```
- **Explanation:** Provides information about the browser and system environment, including user agent, platform, language, etc.

## `window.screen`
- **Example:**
  ```javascript
  console.log("Screen width:", window.screen.width);
  console.log("Screen height:", window.screen.height);
  ```
- **Explanation:** Provides information about the user's screen, including width, height, pixel depth, and orientation.

## `window.scroll()`
- **Example:**
  ```javascript
  window.scroll({
    top: 0,
    left: 0,
    behavior: 'smooth'
  });
  ```
- **Explanation:** Scrolls the window to the specified coordinates, optionally with smooth animation.

## `window.scrollBy()`
- **Example:**
  ```javascript
  window.scrollBy({
    top: 100,
    left: 0,
    behavior: 'smooth'
  });
  ```
- **Explanation:** Scrolls the window by the specified amount, optionally with smooth animation.

## `window.scrollX` / `window.scrollY`
- **Example:**
  ```javascript
  console.log("Horizontal scroll position:", window.scrollX);
  console.log("Vertical scroll position:", window.scrollY);
  ```
- **Explanation:** Returns the current horizontal and vertical scroll positions of the window, in pixels.

## `window.scrollMaxX` / `window.scrollMaxY`
- **Example:**
  ```javascript
  console.log("Maximum horizontal scroll position:", window.scrollMaxX);
  console.log("Maximum vertical scroll position:", window.scrollMaxY);
  ```
- **Explanation:** Returns the maximum possible horizontal and vertical scroll positions of the window, in pixels.

## `window.scrollIntoView()`
- **Example:**
  ```javascript
  const element = document.getElementById("target");
  element.scrollIntoView({ behavior: 'smooth' });
  ```
- **Explanation:** Scrolls the window to bring the specified element into view, optionally with smooth animation.

## `window.resizeTo()`
- **Example:**
  ```javascript
  window.resizeTo(800, 600);
  ```
- **Explanation:** Resizes the window to the specified width and height, in pixels.

## `window.resizeBy()`
- **Example:**
  ```javascript
  window.resizeBy(100, 50);
  ```
- **Explanation:** Resizes the window by the specified amount relative to its current size, in pixels.

## `window.getSelection()`
- **Example:**
  ```javascript
  const selection = window.getSelection();
  console.log("Selected text:", selection.toString());
  ```
- **Explanation:** Returns a Selection object representing the currently selected text in the document.

## `window.getSelection().modify()`
- **Example:**
  ```javascript
  const selection = window.getSelection();
  selection.modify('extend', 'backward', 'character');
  ```
- **Explanation:** Modifies the selection by moving the selection focus in a specified direction.

## `window.getSelection().collapse()`
- **Example:**
  ```javascript
  const selection = window.getSelection();
  selection.collapse(document.body, 0);
  ```
- **Explanation:** Collapses the selection to the start or end of a specified node.

## `window.getSelection().extend()`
- **Example:**
  ```javascript
  const selection = window.getSelection();
  selection.extend(document.body, 10);
  ```
- **Explanation:** Extends the selection to a specified node and offset within that node.
