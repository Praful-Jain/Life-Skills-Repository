# Technical Paper


## Aim
How does a browser render HTML, CSS, and JS to a DOM? What is the mechanism behind it?


## Abstract
Browser rendering is the process through which web browsers convert HTML,CSS, and JavaScript code into the visual representation of a web page. This paper provides an in-depth explanation of the process underlying browser rendering, highlighting the critical stages from the initial parsing of HTML to the final composition of the visual layout.


## Introduction
The exponential growth of the internet has transformed the way we interact with information, services, and applications. And a major credit for this exponential growth goes to browser rendering, which plays a significant role in translating web code into visually engaging and interactive experiences for users.


## Understanding the Browser Rendering Process
It includes a few steps:
- Process HTML markup and build the DOM tree.
- Process CSS markup and build the CSSOM tree.
- Combine the DOM and CSSOM into a reader tree.
- Run the layout on the render tree to compute the geometry of each node.
- Paint the individual nodes on the screen.


## Rendering Engine
It is the part that parses the HTML and CSS in JavaScript, and based on the results, it’s going to display the page. The rendering engine is a core software component of every major browser, and different browser manufacturers call their engines by different names. The browser engine for Firefox is called Gecko, and Chrome’s is called Blink, which happens to be a fork of WebKit.

BASIC RENDERING ENGINE FLOW:
![image](https://github.com/Praful-Jain/Life-Skills-Repository/assets/65565414/0886e3a9-f08d-4f47-a3e4-b789e52b8e92)
              

The rendering process includes several key steps:

### 1. Parsing
The browser parses the HTML markup to understand the structure of the webpage. It creates a Document Object Model (DOM) tree, which represents the hierarchical structure of the HTML elements.
### 2. CSS Styling
The browser then processes the CSS stylesheets associated with the HTML document. It computes the final styles for each element, taking into account factors such as inheritance, specificity, and the cascade of styles.
### 3. Layout
Based on the computed styles, the browser calculates the layout of each element, determining their position and size relative to the viewport and other elements on the page. This process is often referred to as the "reflow" or "layout" phase.
### 4. Painting
Once the layout is determined, the browser paints the pixels on the screen according to the computed styles and layout. This involves filling in the colors, borders, and textures of the elements.
### 5. Composition
The browser combines all the painted elements to create the final representation of the webpage, taking into account layers, stacking contexts, and other visual properties.


## Browser Rendering Optimization 
Efficient browser rendering is crucial for delivering a smooth and responsive user experience. To optimize rendering performance, various techniques are employed, such as minimizing the use of complex CSS selectors, reducing the number of reflows and repaints, and leveraging browser-specific optimizations and hardware acceleration.

### Techniques:

### 1. Minimize HTTP requests
Reducing the number of HTTP requests needed to load a page can significantly improve website speed. This can be achieved by combining multiple CSS and JavaScript files into a single file, reducing the number of images on a page, and using CSS sprites to reduce the number of image requests.

### 2. Optimize images
Compressing images can significantly reduce the file size, leading to faster load times. Appropriate image formats, such as JPEG for photographs and PNG for graphics, can also improve website speed. You can insert image links in the web pages to minimize image load in your website. 

### 3. Use a Content Delivery Network (CDN)
CDNs can help improve browser rendering performance by caching website content closer to the user. This means that when the user visits the website, the content can be retrieved more quickly, resulting in a faster and more responsive website experience. 

### 4. Reduce server response time
Server response time refers to the amount of time it takes for the server to respond to a user’s request. A slow server response time can significantly impact website speed. One way to reduce server response time is to optimize server-side code, such as database queries, to ensure that they execute quickly. 

### 5.Minimize CSS and JavaScript
Large CSS and JavaScript files can slow down website speed, as they increase the amount of data that needs to be downloaded by the user’s browser. Minimizing CSS and JavaScript files by removing unused code, compressing files, and using minification tools can improve website speed. Besides, placing CSS files in the header and JavaScript files at the bottom of the page can help to improve website speed by allowing the browser to render the page faster.


## Conclusion
To sum up, understanding how web pages are shown on your screen is complex. We discussed how browsers change code into what you see, like understanding the code, deciding how things should look, and then actually making it look that way. It's important for websites to load quickly and look the same for everyone, so we talked about ways to make that happen. By following these ideas, websites can work better for everyone, no matter what device they use.


## References
- [How browser rendering works](https://blog.logrocket.com/how-browser-rendering-works-behind-scenes/)
- [Kruno: How browsers work | JSUnconf 2017](https://www.youtube.com/watch?v=0IsQqJ7pwhw)
- [Understanding Browser Rendering Process | ReactJS Bootcamp](https://www.youtube.com/watch?v=waF8xbjJcFU)
- [The rendering engine and tips to optimize its performance](https://medium.com/sessionstack-blog/how-javascript-works-the-rendering-engine-and-tips-to-optimize-its-performance-7b95553baeda)
- [Browser Rendering Optimization](https://blog.eazyplugins.com/browser-rendering-optimization-for-website-speed/)

