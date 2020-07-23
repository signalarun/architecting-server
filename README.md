# architecting-server
Notes on server architecture focusing on ASR - Scalability, Performance and Security


## Service Level Agreement
 ![SLA chart](./resources/SLA%20chart.png)
 
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
## Issues
* c10k problem

## Servers
 * Nginx
    “a free, open-source, high-performance HTTP server and reverse proxy, as well as an IMAP/POP3 proxy server .” Nginx is known for its high performance, stability,
    rich feature set, simple configuration, and low resource consumption.You can consider Nginx as event-based reverse proxy server.
 * Node.js
 * Apache

