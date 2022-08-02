# RESTful API

REST is a **protocol-agnostic** architectural style that was suggested by *Fielding* for building distributed systems (clients decoupled from server).

REST APIs are designed around *resources*, which are any kind of *object, data, or service* that can be accessed by the client; a resource has an *identifier* a URL that uniquely identify the resource, ex:
><https://adventure-works.com/orders/1>

with REST APIs the programmer uses verbs for the HTTP methods, the most common verbs are:

- **GET**

- **POST**

- **PUT**

- **PATCH**

- **DELETE**

In order for a service or API to be effectively RESTful, it must adhere to the following constraints:

- *Client-server*

- *Stateless*

- *Cacheable*

- *Layered system*

- *Uniform interface: resources identification, resources representation, self-descriptive messages, hypermedia*

Another factor is that all web requests impose a load on the web server. The more requests, the bigger the load. Therefore, try to avoid "*chatty*" web APIs that expose a large number of small resources.
