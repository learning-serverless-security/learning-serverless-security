# Learning Serverless Security

This is the code repository for the book *Learning Serverless Security*, published by O'Reilly.

![Learning Serverless Security](book-cover.png)

## Chapter 1: Introduction to Serverless Computing

In this chapter, you will learn what serverless is, along with other key concepts relevant to serverless architectures. You will explore scenarios where serverless makes the most sense and examine and debunk various myths and misconceptions associated with serverless computing. Toward the end of this introductory chapter, you will also discover that serverless applications are not immune to security threats and risks.

## Chapter 2: Understanding Serverless Architectures and Implementation Patterns

In this chapter, you will explore various cloud services and capabilities that enable the serverless operational model. You will dive deep into some of the most common building blocks, patterns, and solutions used in serverless architectures and review the relevant security considerations along the way.

## Chapter 3: Diving Deeper into Serverless Security Threats and Risks

In this chapter, you’ll dive deeper into serverless security threats and risks and examine how these could lead to breaches and incidents. You will learn how attackers adapt their techniques to serverless implementation patterns and exploit vulnerabilities and misconfigurations in the building blocks and services used within serverless architectures.

## Chapter 4: Exploiting and Securing Exposed AWS IAM Credentials

In this chapter, you will examine how attackers can exploit exposed IAM credentials in serverless applications. You will dive deep into how credentials in client-side code can be abused to gain full administrative access to an AWS account, how overly permissive IAM policies can be leveraged to disable AWS CloudTrail logging, and how backdoor IAM users can be created with just a few commands. Toward the end of the chapter, you will learn how to audit CloudTrail event data and Bedrock model invocation logs to investigate security incidents and understand how attacks unfold in a serverless application.

**Chapter Resources**: 

- **Gist**: [Chapter code & commands](https://gist.github.com/learning-serverless-security/0473eb5e8ca1017c0b95935ad70a46e6)
- **Github Repository**: [exposed-credentials-chat-example](https://github.com/learning-serverless-security/exposed-credentials-chat-example)

## Chapter 5: Exploiting and Securing Misconfigured AWS IAM Roles

In this chapter, you'll explore how attackers can perform privilege escalation by using misconfigured AWS IAM roles. You'll also see how they might establish persistence by deploying a backdoored version of a Lambda function to regain access even after credentials are rotated or revoked.

**Chapter Code & Commands**: [View the Gist](https://gist.github.com/learning-serverless-security/b17727f3b7a61ea2375a54efc99b1f86)

## Chapter 6: Hacking Publicly Accessible AWS Lambda Functions

In this chapter, you will take a closer look at how attackers can exploit publicly exposed vulnerable Lambda functions. You'll experience the attacker’s perspective firsthand and execute arbitrary code to retrieve the source code of the compromised Lambda function, as well as exfiltrate credentials from within the serverless application. This will help you recognize security issues and misconfigurations before they can be exploited.

**Chapter Resources**: 

- **Gist**: [Chapter code & commands](https://gist.github.com/learning-serverless-security/219fae2eb40b4c55bbf657eda7af100b)
- **Github Repository**: [vulnerable-lambda-function-backend](https://github.com/learning-serverless-security/vulnerable-lambda-function-backend)

## Chapter 7: Running and Securing Serverless Functions in a VPC

In this chapter, you'll build on what you've learned and configure the Lambda function with a VPC with restrictive outbound access. You will also refactor the function code to eliminate the use of eval() to secure it against code injection attacks. As you dive deeper into the next chapter, you'll learn which security controls are effective and which ones fall short against the types of attacks leveraged by attackers in serverless applications.

**Chapter Code & Commands**: [View the Gist](https://gist.github.com/learning-serverless-security/b64e27b3ae3b45fbad9684f50218c36d)

## Chapter 8: Hacking and Securing Google Cloud Storage Buckets

In this chapter, you will shift your focus to Google Cloud and explore how attackers can exploit cloud storage bucket misconfigurations to expose or steal sensitive data. You will simulate scenarios such as dangling bucket takeovers and examine how lingering references to deleted buckets can be abused for malicious purposes. Finally, you will learn how to enforce secure bucket configurations by using IaC to minimize the risk of costly misconfigurations.

**Chapter Code & Commands**: [View the Gist](https://gist.github.com/learning-serverless-security/8d68b9283896610f573fc38022da6cdc)

## Chapter 9: Abusing Google Cloud Storage Event Triggers with Malicious File Uploads

In this chapter, you’ll dive deeper into how attackers exploit misconfigurations and code injection vulnerabilities in event-driven file-processing applications in Google Cloud. You’ll also examine what works and what doesn’t when securing event-driven file-processing workflows from attackers.

**Chapter Code & Commands**: [View the Gist](https://gist.github.com/learning-serverless-security/488fee2baadda2c37c72db84004669bf)

## Chapter 10: Setting up Backdoors and Escalating Privileges in Google Cloud

In this chapter, you will build on what you’ve learned by exploring how an attacker could exploit a vulnerable Cloud Run service, bypass restrictions, and set up a backdoor without relying on a reverse shell. You will also simulate privilege escalation in Google Cloud by abusing overly permissive service accounts tied to serverless compute resources.

**Chapter Code & Commands**: [View the Gist](https://gist.github.com/learning-serverless-security/f3be4ec4e33abae6053f69f3ae41b126)

## Chapter 11: Hacking and Securing Azure Functions

In this chapter, you’ll shift your focus to Microsoft Azure and examine how attackers can exploit vulnerable Azure Functions. As you go through the simulations and hands-on examples, you’ll learn how to recognize various types of misconfigurations and secure them against potential threats.

**Chapter Code & Commands**: [View the Gist](https://gist.github.com/learning-serverless-security/7b55190a065e175a9cf8f4df0d2ca88c)

## Chapter 12: Escalating Privileges in Microsoft Azure

In this chapter, you will dive deep into privilege escalation in Azure by examining how an overly permissive managed identity tied to the vulnerable function app can be abused. You’ll simulate extracting the function app’s managed-identity access token, then use that token to escalate to Owner-level privileges and read secrets from Azure Key Vault.

**Chapter Code & Commands**: [View the Gist](https://gist.github.com/learning-serverless-security/f1db55c6a67c2a69790f0df9ebab0412)

## Chapter 13: Analyzing, Auditing, and Securing Serverless Application Code

In this chapter, you will explore additional techniques and best practices to secure your serverless applications. You’ll learn how to leverage automated tools, secure coding practices, and custom scripts to further secure your applications against code injection, supply chain attacks, and other emerging threats.

**Chapter Code & Commands**: [View the Gist](https://gist.github.com/learning-serverless-security/ba892f00ce67dd5748af7f5c3ef1ace8)


## Get to Know the Author

**Joshua Arvin Lat** is the Chief Technology Officer (CTO) of NuWorks Interactive Labs, Inc. He previously served as the CTO of three Australian-owned companies and as the Director for Software Development and Engineering for multiple ecommerce start-ups. Years ago, he and his team won first place in a global cybersecurity competition with their published research paper. He is an AWS AI Hero and has authored several other technical books including Machine Learning with Amazon SageMaker Cookbook, Machine Learning Engineering on AWS, and Building and Automating Penetration Testing Labs in the Cloud. Because of his proven track record in leading digital transformation within organizations, he has been recognized as one of the prestigious Orange Boomerang: Digital Leader of the Year 2023 award winners.


## Other books by the author

* [Machine Learning Engineering on AWS](https://www.packtpub.com/product/machine-learning-engineering-on-aws/9781803247595)

* [Machine Learning with Amazon SageMaker Cookbook](https://www.packtpub.com/product/machine-learning-with-amazon-sagemaker-cookbook/9781800567030)
  
* [Building and Automating Penetration Testing Labs in the Cloud](https://www.packtpub.com/product/building-and-automating-penetration-testing-labs-in-the-cloud/9781837632398)
