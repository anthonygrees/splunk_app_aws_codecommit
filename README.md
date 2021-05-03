# Splunk App - AWS CodeCommit
  
### Introduction
AWS CodeCommit is a fully-managed source control service that hosts secure Git-based repositories. It makes it easy for teams to collaborate on code in a secure and highly scalable ecosystem. CodeCommit eliminates the need to operate your own source control system or worry about scaling its infrastructure.  
  
### The Splunk App
This is a `demo` Splunk App to display the transactions from AWS Web CodeCommit.  It is not supported by Splunk and is a template guide for customers or partners to enhance, extend and develop further.  
  
Feel free to `fork` this code repo and modify it for your own needs.  Should you have feature requests, or find bugs, please raise the [issues here](https://github.com/anthonygrees/splunk_app_aws_codecommit/issues) and log them so they can be tracked.  
  
### Getting Data In (GDI) - Lambda CodeCommit
[Lambda CodeCommit](https://github.com/anthonygrees/lambda_codecommit) application is designed to be a generic approach for collecting AWS CodeCommit events and forwarding them onto a HEC (HTTP-Event-Collector) Endpoint in Splunk.  
  
The Lambda CodeCommit application will create a lambda function, with an API Gateway trigger. When deployed, you can use the API Gateway UR and "webhook-to-hec" endpoint, along with Environment Variables, to send data from AWS CodeCommit into Splunk.  
  
### What the App looks like
The app is a demo application that can be extended for customer or partner needs.  
  
![CodeCommitApp](/images/ui.png)
  
### Install It
Download the `aws-codecommit-app_001.tgz` file onto your Splunk Server and run the command:  
```bash
splunk install app /tmp/aws-codecommit-app_001.tgz -auth user:password
```  
  
## License and Author
  
* Author:: [Anthony Rees](<reesy@splunk.com>)

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.