# Network Questions:

* Traditionally, why has it been better to serve site assets from multiple domains?
Parallelization

Reduced header overhead


* Do your best to describe the process from the time you type in a website's URL to it finishing loading on your screen.


Step 1 -->  Get the ip address of the URL.

To Get the IP address for http://www.quora.com, the steps are
a) System checks the browser cache. Browser caches the DNS data for some time.
b) If IP address[DNS data for http://www.quora.com]   is not found in browser cahe, system will check the OS cache. [in windows gethostbyname system call is made]
c) If IP address[DNS data for http://www.quora.com] is not found in  OS cache, then  request continues to DNS cache maintained by the router.
d) If DNS data for http://www.quora.com is not found then seach moves to next level where DNS cache of your Internet Service Provider.
e) If the  DNS data is not found in ISP's DNS cache, then ISP's DNS server perform DNS query to search for the required DNS data.


Step 2>> Once browser gets the IP address it opens TCP connection and sends HTTP request to  the web server.

Step 3>> The web server will handle the request [it happens in multiple steps] and send the HTTP response to the client/browser.

Step 4>> The browser parse the HTML docuemnt and render it.



This is basically summary of what happend when we type an URL and hit enter.

* What are the differences between Long-Polling, Websockets and Server-Sent Events?


https://stackoverflow.com/questions/11077857/what-are-long-polling-websockets-server-sent-events-sse-and-comet






* Explain the following request and response headers:

  * Diff. between Expires, Date, Age and If-Modified-...
  
  
  * Do Not Track
  
  
  
  
  * Cache-Control
  
  The Cache-Control general-header field is used to specify directives for caching mechanisms in both requests and responses. Caching directives are unidirectional, meaning that a given directive in a request is not implying that the same directive is to be given in the response.
  
  
  
  * Transfer-Encoding
  
  The Transfer-Encoding header specifies the form of encoding used to safely transfer the entity to the user.
  
  
  
  * ETag
  
  An ETag is an opaque identifier assigned by a web server to a specific version of a resource found at a URL. If the resource representation at that URL ever changes, a new and different ETag is assigned. Used in this manner ETags are similar to fingerprints, and they can be quickly compared to determine whether two representations of a resource are the same.
  
  
  
  * X-Frame-Options
  
  The X-Frame-Options HTTP response header can be used to indicate whether or not a browser should be allowed to render a page in a <frame>, <iframe> or <object> . Sites can use this to avoid clickjacking attacks, by ensuring that their content is not embedded into other sites.
  
  
  
  
  
* What are HTTP methods? List all HTTP methods that you know, and explain them.


https://www.tutorialspoint.com/http/http_methods.htm
