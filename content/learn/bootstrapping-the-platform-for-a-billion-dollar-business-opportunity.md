---
title: Bootstrapping the Platform for a Billion Dollar Business Opportunity
description: "How SC5 used Serverless to help MaaS revolutionize transportation"
layout: Default
---

# Bootstrapping the Platform for a Billion Dollar Business Opportunity

### Background

SC5, based in Helsinki, is a digital agency specializing in cloud solutions.
The SC5 team works with enterprise clients to create cloud-native apps,
APIs and data solutions. The team recently helped build the backend for the
award-winning Whim personal transportation app by MaaS Global.

<a href="http://maas.global" target="_blank">MaaS Global</a> (Mobility as a
Service) is a startup working to revolutionize personal transportation.
Supported by the increasing trends of urbanization and buying everything as a
service, we travel more, but we don't want to own a car.

<a href="http://whimapp.com/fi-en" target="_blank">Whim</a> – the mobile
application by MaaS Global, has been called the "Spotify of transportation".
Whim offers a wealth of options from getting place A to B by public transport,
taxi and even rental car – all in a digital subscription service.

<img src="https://s3-us-west-2.amazonaws.com/assets.site.serverless.com/partners/maas-whim-app.png" alt="MaaS Whim app" />

### The Challenge

There are no common standards and few business practices on how
to order buses, taxis or rental cars on behalf of the end customers. MaaS had to
create its own models, and adapt their model to fit to the varying practices
and IT systems of its partners.

Instead of creating its own maps, geodata or routing systems, MaaS aimed to tap
into the existing systems in the field. The technical challenge was making them
work together reliably while supporting potentially millions of concurrent users.

SC5 constructed the technical backbone of this system, so that it could be proven
to the investors and partners, and helped MaaS developers get up-to-speed with
Serverless development on AWS.

### The Solution

SC5, in co-operation with the MaaS development team, applied their Serverless
know-how and constructed a microservices architecture consisting of a few dozen
adapters with its own data storage for order handling. The system was founded on
AWS services, consisting of a REST API using the Serverless Framework and Postgres
data storage. With the exception of managed database services, the whole solution
was based on a serverless architecture pattern with Lambda and API Gateway, which
theoretically scales infinitely out-of-the-box.

Because the technical mash-up of external maps, geocoding, routing and booking
services could fail if any of the third party services fail, some practices to
increase fault tolerance were taken into account. A continuous integration
system was built using GitHub and Travis, so that new development could happen
without exhaustive manual integration and testing work.

<img src="https://s3-us-west-2.amazonaws.com/assets.site.serverless.com/partners/maas-architecture.png" alt="MaaS architecture" class="right" />

### Why Serverless

SC5 chose the Serverless Framework because they had prior experience with
the framework and its predecessor (JAWS), and it was the most robust framework
for developing serverless applications on AWS. The framework also provided a
plug-in mechanism. This helped to streamline the build and deploy process for
optimal output and application performance.

### Results

The first end-to-end version, consisting of the full flow of finding a route
through getting a Taxi ordered was demoed to investors just four months after the
start of the project. Since then, the platform has launched in beta in the Helsinki
area with paying end customers, and it' s currently expanding internationally to the
United Kingdom.

Creating a Serverless backend allowed developers to focus on building application
logic instead of operating the infrastructure. This is the same reason why
companies like Zalando are operating their stack in the cloud.

The Whim app, powered by the SC5 bootstrapped backend has won several awards,
including the Helsinki Smart City Action Award and Nordic Smart Cities Award. Whim
has been featured in the international press, including *The Economist*, *The
Guardian*, *Wired* and *Helsingin Sanomat*.

Eight months after the start of the project, new development still stands
on the same foundations set in the bootstrapping phase. MaaS has
successfully passed all planned steps of funding, is in a public beta phase in
the Helsinki area, and is currently expanding to the first locations outside
of Finland. An internal development team capable of taking over the task of
developing the solution further was successfully ramped up during the project.

<blockquote>SC5 was our choice for this project because of their expertise in
cloud solutions and Serverless microservices. We needed Whim-app to be
extendable and scale arbitrarily straight from the start.  The whole process was
really fast-paced and results spectacular; first online routing demo with a test
site was up overnight, surprising everyone in the industry and even our board,
making the CTO look good in the process!<br/>
<b>Sami Pippuri</b> - <i>CTO at MaaS Global</i> </blockquote>

"The serverless architecture and Serverless Framework have been a perfect fit
for us. The serverless architecture allows developers to focus on actual
business logic instead of the black magic involved in classical backend
solutions. This has helped us to lower the bar in enabling frontend developers
to go fullstack and contribute to the backend application as well.”, SC5 CTO
Mikael Puittinen. He adds: ”The serverless framework allows us to automate the
development lifecycle from project creation to deployment and operations. Its
open plugin architecture allows developers such as us to extend the platform
with functionality that streamlines the development lifecycle even further."

### About us (SC5):

We create cloud native applications and solutions that allow you to serve your
customers faster, better and more cost-efficiently. We are experts in the
latest serverless technologies, user centric design and web UI development and
have a track record of over 400 customer projects. SC5 was founded in 2006.

We are an AWS Lambda, API Gateway and DynamoDB APN Partner.

### Serverless contributions by SC5

* https://github.com/SC5/serverless-boilerplate : a boilerplate project for the
  serverless framework, which incorporates optimized deployment and commands for
  test driven development
* https://github.com/SC5/serverless-mocha-plugin : a plugin for creating
  functions, test cases and invoking tests
* https://github.com/SC5/serverless-authentication-boilerplate : a boilerplate
  for creating API gateway custom authorizers
* https://github.com/SC5/serverless-messenger-boilerplate : a boilerplate for
  creating Messenger / Wit.ai bots
* http://serverless.fi : Serverless Finland community
* http://serverless.fi/docs/bot-workshop.pdf : a step-by-step workshop for
  creating a simple serverless blog backend using the Serverless framework
* http://serverless.fi/docs/messenger-workshop.pdf : a step-by-step workshop for
  creating a weather bot on Messenger using the Serverless framework. Featured
  in ServerlessConf London 2016
