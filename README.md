# GDSC Cloud Task
This is a repository dedicated to the task(s) provided by the Google Development Students Community, particularly for its Cloud Domain

## A Case Study on the topic: **Monolith vs Serverless**

There are different ways of building applications and there isn't any perfect way. But there are ways to ensure the path taken to build software products, is as hassle-free and efficient as possible depending on the application type, its needs, and the customer/user it targets. At the end of this case study, I expect to be much clearer about my vision and find the most favorable way for my app to function behind the scenes.

> The style I chose for writing this case study is a comparative one which stacks both paths against each other for a crystal clear view of both, and why you might have to  choose one over the other depending on the use case. 



### Architecture

#### Monolith
![Monolith architecture diagram](https://res.cloudinary.com/practicaldev/image/fetch/s--DLcP9_Fn--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_800/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/w9jf2w448vgnued8pt23.png)

A monolith server-side app — also known as a monolith, is an application delivered via a single deployment, it is also available in one single endpoint and all required logic exists there. A single database is linked with the front end through a single backend route that creates a simplistic pathway for data flow at/to a single instance. 


 #### Serverless
![Serverless architecture diagram](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*XNkYt06HmRN5GKYD5ymuJA.jpeg)

A serverless architecture — also known as serverless computing or function as a service (FAAS), is a software design pattern where our function (a part of the microservice responsibility) is hosted by a third-party service (AWS Lambda functions, Azure functions, Firebase cloud functions, etc…), this architecture eliminates the need for server software and hardware management by the developers, the third-party service provides this automatically. The architecture as a whole depends on the service provider subscribed to, i.e., a monolith or a microservice structure (preferably microservice) which is entirely dealt with and taken care of by the service, such as AWS, Azure, Google Cloud Platform(GCP), etc.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Ease of Development and Debugging

#### Monolith
The monolithic structure is easier to build as a beginner because of the presence of a central location for all the source code which makes it easy to understand.
But as the project grows it gets tougher to manage the codebase as there is a lack of any proper boundary between tasks allocated to modules, thus for a new team of developers coming in, it can turn into quite a headache to familiarise with the codebase and identify the bugs and other issues as they are. Faster development than a custom-developed microservices architecture, but may or may not be faster than a serverless architecture.


#### Serverless
Fast development because less configuration is needed.  No infrastructure or OS needs to be maintained leading to fewer problems and developers do not need to care about scaling, the third-party software does it automatically. Multiple languages are available, and every function can be written in any language suitable for that task.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Cost

#### Monolith
Early on in the application, costs are low. One deployment unit, containing all the source code is created, packed, and deployed. But as the project goes out of the MVP phase and moves on to the usability/marketability phase, the scalability of the structure comes into question and for this very reason, monolith projects are suggested to be designed as modular as possible. 


#### Serverless
You only pay for the requests made, so you are not paying for servers or virtual machines that aren't being used. If the product is to be released by a non-developer, they might save money by not needing to recruit and pay a developer to take on the same tasks that are cheaply outsourced to services such as AWS Lambda, Firebase Cloud Platform by Google and so on.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Testing

#### Monolith
Test a single service independently of any dependencies. Usually, everything is obvious and the task is simple to execute in most cases. In case issues are found, fixing them might be completely dependent on the creators's company and not on any other service.

#### Serverless
Unit tests may be conducted on function code by developers, but integration tests, which assess how frontend and backend components interact, are challenging to execute as a large part of the backend code lies in the hands of the service vendors.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Security

#### Monolith
If you change something in one service, it could break another service’s functionality because they were tightly coupled together without any abstraction layers in between them (e.g., no interfaces between them). This same interface which seems troubling results in a tightly set secure network within the system, unlike microservices where multiple services require multiple routes for data to flow freely within the interconnected system of services, resulting in the exposure of data for hackers to take advantage of.

#### Serverless
A cloud provider might run code from a few of its clients simultaneously on the same server. Your application data may be exposed if the shared server is improperly set up. So the control of security of your product lies in the hands of the service providers.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Control

#### Monolith
All of the data lies in the personal database and servers, hence the flow of data can be controlled according to the needs of the developers.

#### Serverless
You have no control over the software stack that your code uses in serverless settings. You must rely on a cloud provider to resolve any problems that affect one of your servers due to hardware failure, data center outage, or other problems. Big cloud providers like AWS provide a variety of services, including APIs, messaging queues, and databases, which can all be used together to build serverless applications. Although components from several vendors can be combined, services from a single provider are made to integrate most easily. So, you are directly or indirectly forced to lay all the important data of your product into the hands of large capitalist firms and companies without any further control of it.
