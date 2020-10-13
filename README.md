"The difference between a good designer and a great designer is the ability to not only solve the problem, but also to articulate how the design solves it in a way that is compelling and fosters agreement. If you can do that, you’re a great designer." - Articulating Design decisions

The NIST has claimed, based on a study of popular web applications, that “The cost of removing an application security vulnerability during the design phase ranges from 30–60 times less than if removed during production.” - Web Application Security by Andrew Hoffman

# architecting-server
Notes on server architecture focusing on ASR - Scalability, Performance and Security

## Functionalities
 * SSL termination
 * Load balancing
 * Extend monitoring and logging
 * Decoupling Web application server from frontend server ie shifting actitivies like managing incoming traffic to frontend server
   - SSL termination
   - Efficient handling of static files
   - Rate, request and connection limiting
   - Caching response from upstream
   - Compressing response from upstream

## Key concepts
 * Cookie
    According to https://web.archive.org/web/20070805052634/http://wp.netscape.com/newsref/std/cookie_spec.html, "Cookies are a general mechanism which server side connections (such as CGI scripts) can use to both store and retrieve information on the client side of the connection. The addition of a simple, persistent, client-side state significantly extends the capabilities of Web-based client/server applications. A server, when returning an HTTP object to a client, may also send a piece of state information which the client will store. Included in that state object is a description of the range of URLs for which that state is valid. Any future HTTP requests made by the client which fall in that range will include a transmittal of the current value of the state object from the client back to the server. The state object is called a cookie, for no compelling reason."

## Service Level Agreement
 ![SLA chart](./resources/SLA%20chart.png)
 
## Issues
* c10k problem
* Single point failure

## Servers
 * Nginx
    “a free, open-source, high-performance HTTP server and reverse proxy, as well as an IMAP/POP3 proxy server .” Nginx is known for its high performance, stability,
    rich feature set, simple configuration, and low resource consumption.You can consider Nginx as event-based reverse proxy server.
 * Node.js
 * Apache
 * Django framework
 
 ## Persistance
 * [NOSQL data modeling techniques](https://highlyscalable.wordpress.com/2012/03/01/nosql-data-modeling-techniques/)

