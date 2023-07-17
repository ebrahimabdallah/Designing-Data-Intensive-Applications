# Chapter One

* In this chapter, we will start by exploring the fundamentals of what we are trying to
achieve: reliable, scalable, and maintainable data systems

* **A data-intensive** application is typically built from standard building blocks that pro‐
vide commonly needed functionality
- This apps which needs these terms:

1-databases:-store data to user 

2-caches:- Remember the result of an operation

3- search indexes :-Allow users to search data by keyword or filter it in various ways

4-stream pro‐cessing :-Send a message to another process asynchronously 

5-batch processing:-Periodically  large amount of data

* many database systems with different charac‐
teristics, because different applications have different requirements

# Thinking About Data Systems

1-We think of databases, queues, caches, etc. as being very different categories
of tools.

2- database and a message queue **both** store data for some time
**but** very different access patterns, which means
different performance characteristics, and thus very different implementations

* If you are designing a data system or service a lot of tricky questions arise 

1-How do you ensure that the data remains correct and complete, even when things go wrong internally

2- How do you provide consistently good performance to clients, even when
parts of your system are degraded? 

3-How do you scale to handle an increase in load?
What does a good API for the service look like?

* The developer uses the database api without knowing the implementation

* combines more than data system to achieve a  purpose

# Reliability 
* **definition** continuing to work correctly, even when things go
wrong.
* tolerate the user making mistakes or using the software in unexpected
ways.

* The system prevents any unauthorized access and abuse.

* The app return user expected.
* good enough for the required use case, under the expected
load and data volume

* **How Important Is Reliability?**
* Bugs in business
applications cause lost productivity Even in “noncritical” applications we have a responsibility to our users. 
* There are situations in which we may choose to sacrifice reliability in order to reduce
development cost

# Error Types

* Hardware Faults
* Software Errors
* Human Errors

# Scalability
When increasing the application, what are the ways we deal with the data in it

# Describing Load
* The best choice of parameters
 depends on the architecture of your system
 *  it may be requests per second to a web server  
* the ratio of reads to writes in a database
* the number of simultaneously active users in a chat room 
* the hit rate on a cache

* The problem of followers on Twitter and how to overcome it
1-Posting a tweet simply inserts the new tweet into a global collection of tweets.
When a user requests their home timeline

2- Maintain a cache for each user’s home timeline—like a mailbox of tweets for
each recipient user

# Describing Performance
* when the load increases. You can look at it in two ways:

1- When you increase a load with the same resources , how is the performance of your system
affected?

2- When you increase a load parameter,
what is the cost of resources 
resources you need to increase if you want to keep performance unchanged?



# Latency and response time
 **Latency** is the duration that a
request is waiting to be handled


**Response** time is the total amount of time it takes to respond to a request for service


* **the mean**  not a very good metric if you want to ” response time, because it doesn’t tell you how many users actually experienced
that delay

* **percentiles** is better  If you take your list of response times


# Maintainability
* Most of the cost of the application is not in the initial stage, but after that when a new addition, modification or error correction is needed

* three design principles for software systems

1-**Operability**
Make it easy for system running smoothly


* Operations teams are vital to keeping a software system running smoothly

- Monitoring

- Tracking down the cause of problems

- Keeping software and platforms up to date

- Establishing good practices and tools for deployment

- Preserving the organization’s knowledge about the system

- Maintaining the security of the system  when change

2- **Simplicity**
* Make it easy for new developer to understand the system

* Making a system simpler does not necessarily mean reducing its functionality; it can
also mean removing accidental complexity.

3- **Evolvability**
Make it easy for engineers to make changes to the system in the future
