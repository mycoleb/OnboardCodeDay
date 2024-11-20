IMPORTANT: You need to make YOUR OWN COPY of this document by clicking on File -> Make a Copy.
General Information About Your Project
In your own words, what does the open source project you're working on do? (We know the README file explains it, but these descriptions are often packed with technical jargon. Let us know what you think it does.)

The task involves creating three function templates in PHP by translating existing templates from Node.js. These templates act as reusable starting points for developers to integrate specific functionalities (e.g., payments or AI). To do this, I will need to understand the logic in Node.js implementations and adapt it to PHP while following best practices.

What resources does this open source project have to help you, such as an online chat community or forums? (You'll have support from your mentor, but we want you to take advantage of all your resources!)
Are there specific testing requirements for the PHP templates?
What is the expected directory structure for new PHP templates?
Are there any Appwrite-specific PHP conventions that should be followed?
How should error handling be implemented - should it match Node.js exactly or follow PHP conventions?

How closely should the PHP implementation match the Node.js logic? Are there specific aspects where deviations are encouraged?
Are there particular standards or conventions to follow in Appwrite's PHP code?
Is there a recommended way to test the templates after translating them?
Should I prioritize writing comments or documentation for these templates?


What are the 2 most important frameworks or libraries you think this project is using? Identify a potential learning resource (tutorial or documentation) for each, beyond what you have already covered in onboarding. IMPORTANT: You don't need to read this learning resource yet!
Tutorial/Documentation: "The Complete Guide to Appwrite Functions" on Dev.to (https://dev.to/appwrite/the-complete-guide-to-appwrite-functions-4kb0)
This resource is essential because it provides a comprehensive overview of how to work with Appwrite's serverless infrastructure. It covers how functions are structured, deployed, and integrated with other Appwrite services, which is foundational for this project.
Stripe PHP Library
Tutorial/Documentation: "Building a Subscription Service with Stripe and PHP" on Stripe's official documentation(https://stripe.com/docs/billing/subscriptions/build-subscriptions)
Since Stripe payments are specifically mentioned as an example template, this guide is particularly relevant. It focuses on implementing subscription functionality using Stripe's PHP SDK, which is a common and practical use case for many applications.
Why I Chose These Resources:
The project centers on Appwrite Function templates, so mastering how to work with Appwrite's SDK is fundamental to successfully translating and implementing the templates.
Stripe integration was explicitly mentioned as an example, and payment processing is a high-priority use case in application development, making Stripe's PHP SDK a critical tool to understand.
, I focused on frameworks and libraries directly tied to the task's goals and the ecosystem.



First Meeting Agenda
In your own words, what is the task you've been assigned asking you to do? Avoid technical jargon -- we want to make sure you know what everything means. (If you're not totally sure, what questions do you have? Please be specific, so that we can help you answer them.)
What questions do you have about the issue you've been assigned to?
How closely should the PHP implementation match the Node.js logic? Are there specific places where deviations are encouraged?
Are there particular standards or conventions to follow in Appwrite's PHP code?
Is there a recommended way to test the templates after translating them?

While doing research on your issue, what have you come across that might be helpful?
Appwrite Templates Repository: Provides existing examples of Node.js and PHP templates.
GitHub Wiki or Docs: Might include guides on implementing serverless functions.
PHP Function Templates in Appwrite: Existing examples that can serve as a reference.
Code Review Discussions: Insights from previous template implementations.
Identify at least three "starting points" in the codebase for working on your issue.
Node.js Template Implementations: These files contain the logic to be translated to PHP.
Existing PHP Templates: Reference examples for how PHP templates are structured.
README Files in Appwrite/Templates: Documentation on how to work with function templates.


What questions do you have about the issue you've been assigned to, which you'd like to discuss with your mentor? Questions might be things like:
Why do they want to change a certain behavior?
What does a certain technical term used in the issue mean?
How do several technical terms fit together?
 Important: please do not ask general, open-ended questions (such as "I don't know what the issue is asking"). Your mentor will not be able to help you if you haven't done your own research.
When implementing the PHP version, should I include support for multiple AI providers (like Anthropic, etc.) since the PHP ecosystem might have different common use cases?"

When translating the Node.js webhook template, I notice it uses Express-specific features. Should the PHP implementation use a particular framework's features (like Laravel/Symfony), or should it remain framework-agnostic?
The Node.js Stripe template uses Stripe SDK version 12.x. Should the PHP implementation target the equivalent Stripe PHP SDK version (10.x), or should we use the latest available PHP SDK version?

While doing research on your issue, what have you come across that might be helpful?
Examples could include:
written documentation
certain files which seem helpful
other issues on Github
"how-tos" and tutorials

Node.js Template Implementations: These files contain the logic to be translated to PHP.
Existing PHP Templates: Reference examples for how PHP templates are structured.
README Files in Appwrite/Templates: Documentation on how to work with function templates.
https://www.youtube.com/watch?v=OK_JCtrrv-c


Identify at least three "starting points" in the codebase for working on your issue. These could be a file or a method you think are involved in solving the issue you're assigned to. Do your best, but it's not important for you to be correct.
templates/node/stripe-payment/src/index.js
This would be the primary reference for the Stripe payment template implementation
Critical to understand the payment flow and required Stripe SDK methods
Shows how environment variables and configuration are handled
Demonstrates proper error handling patterns for payment processing
templates/php/shared/composer.json
Essential for understanding PHP template dependencies structure
Shows which base packages are required for all PHP templates
Helps understand version requirements and constraints
Will need this to add Stripe/other external dependencies correctly
templates/php/[any-existing-template]/src/index.php
Provides the standard entry point structure for PHP templates
Shows how response formatting is handled
Demonstrates error handling patterns specific to PHP templates
Reveals how environment variables and configuration are managed in PHP context


[AFTER THE MEETING] After your conversation with your mentor, in your own words, what are the next steps you should be taking on your project?

First Setup Steps: 

Clone the Appwrite templates repository 
b. Navigate to the README file to get the full list of templates 

c. Create a spreadsheet or note with two columns: - 

Available Node.js templates - Existing PHP implementations 

Template Analysis: 

a. Go through each Node.js template directory 
b. Check the PHP templates directory for matching implementations 
c. Make a list of Node.js templates that don't have PHP versions 
d. Note the complexity and dependencies of each potential template 

Selection Criteria: 

a. For each candidate template, evaluate: 

- my familiarity with the tools/services it uses 
- The complexity of the Node.js implementation 
- The availability of PHP libraries for required services 
- Dependencies and setup requirements Repository Setup: 

a. Create a new branch for my work 
b. Set up my PHP development environment 
c. Look at existing PHP templates for: - 
Directory structure - composer.json pattern - Common code patterns
