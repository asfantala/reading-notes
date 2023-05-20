# Reading : Serverless Functions

### What are the key characteristics of serverless computing, and how does it differ from traditional server-based architectures?

- characteristics of serverless computing include:

   - No server management: Developers can focus on writing application code while the cloud provider handles the infrastructure.

   - Event-driven execution: Applications are triggered by specific events or requests, and functions are executed in response to these events.

   - Automatic scalability
   - Stateless execution: Functions do not maintain persistent server-side state between invocations.
- differs from traditional server-based architectures

|Characteristic|Serverless Computing	|Traditional Server-Based Architectures|
|-|-|-|
|Server Management|No need to provision or manage servers|Manual provisioning and management of servers|
|Scalability	|Automatic scaling up and down based on workload	|Manual scaling of servers|
|Cost Model|Pay-per-use pricing based on execution time and resources|Paying for servers and infrastructure regardless of usage|
|State Management|Stateless execution of functions|Relying on maintaining server state|
|Development Focus|Emphasis on writing application logic|Need to manage low-level infrastructure concerns|
|Deployment Speed|Rapid provisioning and deployment of applications	|Complex deployment processes and server configuration|
### How can one get started with Vercel, and what are the main steps involved in deploying a serverless function using Vercel?
 - sign up a vercel account and connect git provider 
 - Create and deploy a project
 - Configuring Your Project : You can specify the framework you are using, the build command, and other deployment settings.
 - Assigning a Custom Domain - You can find it right below your Project's name on the Project list:

- Applying Updates via Git
- Deploy serverless functions: To deploy a serverless function, create a directory within your project for the functions. Inside that directory, create a file for your function, such as api.js or hello.js. Write your function code in this file.Deploy the serverless function: Run the vercel command again to deploy the changes, including your serverless function. Vercel will build and deploy the updated project, including the function

### What are APIs, and how can they be utilized in Python applications to access and manipulate data from external sources?
- APIs (Application Programming Interfaces) are sets of rules and protocols that allow different software applications to communicate and interact with each other. They define how different software components should interact, enabling data exchange and functionality integration between application
- APIs can be utilized to access and manipulate data from external sources by making HTTP requests to the API endpoints provided by those sources

### What is the Requests library in Python, and how can it be used to interact with APIs by sending HTTP requests? Can you provide an example of a basic GET request using the Requests library?
- To interact with APIs using the Requests library, you need to install it first. You can install it using pip by running the following command in your terminal or command prompt:
```
pip install requests
```
for example :
after install requests you can import it like this :
```
import requests

# Specify the API endpoint URL
url = "https://api.example.com/data"

# Make the GET request
response = requests.get(url)
```