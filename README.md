# GDSC Cloud Task
This is a repository dedicated to the task(s) provided by the Google Development Students Community, particularly for its Cloud Domain

## A Case Study on the topic: **Monolith vs Serverless**

There are different ways of building applications and there isn't any perfect way. But there are ways to ensure the path taken to build software products, is as hassle-free and efficient as possible depending on the application type, its needs, and the customer/user it targets. At the end of this case study, I expect to be much clearer about my vision and find the most favorable way for my app to function behind the scenes.

> The style I chose for writing this case study is a comparative one which stacks both paths against each other for a crystal clear view of both, and why you might have to  choose one over the other depending on the use case. 




### Architecture
#### Monolith
![Monolith architecture diagram](https://res.cloudinary.com/practicaldev/image/fetch/s--DLcP9_Fn--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_800/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/w9jf2w448vgnued8pt23.png)

A monolith server-side app — also known as a monolith, is an application delivered via a single deployment, it is also available in one single endpoint and all required logic exists there. A single database is linked with the frontend through a single backend route that creates a simplistic pathway for data flow at/to a single instance. 


 #### Serverless
![Serverless architecture diagram](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*XNkYt06HmRN5GKYD5ymuJA.jpeg)

A serverless architecture — also known as serverless computing or function as a service (FAAS), is a software design pattern where our function (a part of the microservice responsibility) is hosted by a third-party service (AWS Lambda functions, Azure functions, Firebase cloud functions, etc…), this architecture eliminates the need for server software and hardware management by the developers, the third-party service provides this automatically. The architecture as a whole depends on the service provider subscribed to, i.e., a monolith or a microservice structure (preferably microservice) which is entirely dealt with and taken care of by the service, such as AWS, Azure, Google Cloud Platform(GCP), etc.


### Ease of Development and Debugging
#### Monolith
The monolithic structure is easier to build as a beginner because of the presence of a central location for all the source code which makes it easy to understand.
But as the project grows it gets tougher to manage the codebase as there is a lack of any proper boundary between tasks allocated to modules, thus for a new team of developers coming in, it can turn into quite a headache to familiarise with the codebase and identify the bugs and other issues as they are. Faster development than a custom-developed microservices architecture, but may or may not be faster than a serverless architecture.


### Serverless
Fast development because less configuration is needed.  No infrastructure or OS needs to be maintained leading to fewer problems and developers do not need to care about scaling, the third-party software does it automatically. Multiple languages are available, and every function can be written in any language suitable for that task.


### Cost
