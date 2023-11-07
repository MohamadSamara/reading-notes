# Read Class 32

**What makes an API RESTful?**

An API (Application Programming Interface) is a set of rules that define how computers can communicate with each other. A RESTful API is an API that conforms to the design principles of the REST, or representational state transfer architectural style.

**Here are some of the key characteristics of a RESTful API:**

* **It uses HTTP as the underlying protocol.** HTTP is a stateless protocol, which means that each request is independent of any other request. This makes RESTful APIs easy to scale and distribute.
* **It uses URIs (Uniform Resource Identifiers) to identify resources.** URIs are unique identifiers for resources on the web. For example, the URI `https://example.com/users/1` identifies the user with the ID 1 on the example.com website.
* **It uses standard HTTP methods (GET, POST, PUT, and DELETE) to perform CRUD operations (Create, Read, Update, and Delete) on resources.** For example, a GET request to the URI `https://example.com/users/1` would retrieve the user with the ID 1, while a POST request to the same URI would create a new user.
* **It returns resources in a standard format.** The most common format is JSON, but XML and other formats are also supported.

**What is the benefit of using GraphQL? Any downsides?**

GraphQL is a query language for APIs that allows developers to request specific data from an API without having to know the underlying schema. This makes it easier to build complex applications that rely on data from multiple APIs.

**Here are some of the benefits of using GraphQL:**

* **Flexibility:** GraphQL allows developers to request exactly the data they need, in the format they need it. This can lead to more efficient and performant applications.
* **Power:** GraphQL can be used to query data from multiple APIs in a single request. This can simplify the development of complex applications.
* **Introspection:** GraphQL provides a built-in introspection feature that allows developers to discover the schema of an API without having to read documentation.

**Downsides of using GraphQL:**

* **Complexity:** GraphQL can be more complex to learn than other query languages, such as REST APIs.
* **Performance:** GraphQL queries can be less performant than REST API requests, especially for complex queries.

**Describe “serverless” to a new 301 Code Fellows student.**

Serverless computing is a cloud computing model in which the cloud provider manages the server infrastructure and dynamically allocates resources to applications based on demand. This allows developers to focus on building and deploying applications without having to worry about managing servers.

**Here is a simple analogy to explain serverless computing:**

Imagine a restaurant where the customers don't have to worry about cooking, washing dishes, or cleaning up. The restaurant staff takes care of all of those tasks for the customers. Serverless computing is similar, but instead of customers and restaurant staff, we have developers and cloud providers.

**Benefits of serverless computing:**

* **Scalability:** Serverless applications can scale automatically to meet demand. This means that developers don't have to worry about provisioning and managing servers.
* **Cost savings:** Serverless applications are only charged for the resources they use. This can lead to significant cost savings for developers.
* **Ease of use:** Serverless computing is a relatively new technology, but it is becoming increasingly easy to use. There are a number of cloud providers that offer serverless computing platforms, such as AWS Lambda, Azure Functions, and Google Cloud Functions.
