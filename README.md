This project is implemented using C and Parsing of HTTP.

##### How did we implement Multi-threading?
Used Semaphore instead of Condition Variables and pthread_join() and pthread_exit() function. 
pthread_join() requires us to pass the thread id of the the thread to wait for.

##### Motivation/Need of Project
To Understand → 
  - The working of requests from our local computer to the server.
  - The handling of multiple client requests from various clients.
  - Locking procedure for concurrency.
  - The concept of cache and its different functions that might be used by browsers.
Proxy Server do → 
  - It speeds up the process and reduces the traffic on the server side.
  - It can be used to restrict user from accessing specific websites.
  - A good proxy will change the IP such that the server wouldn’t know about the client who sent the request.
 
  - ##### OS Component Used  
Threading
Locks 
Semaphore
Cache (LRU algorithm is used in it)

## How to Run

```bash
$ git clone https://github.com/sreejish05/Multithreaded-Proxy-Web-Server.git
$ cd Multithreaded-Proxy-Web-Server
$ make all
$ ./proxy <port no.>
