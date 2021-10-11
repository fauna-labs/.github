Welcome to [Fauna Labs](https://github.com/fauna-labs) - a collection of [tooling](#useful-tooling) and [examples](#helpful-examples) to help you build with Fauna more effectively. From Infrastructure as Code (IaC) tools to single sign-on (SSO) application templates, Fauna Labs has everything you need to deliver applications more quickly with Fauna!

## Useful tooling

Fauna Labs provides tooling to help you manage your databases. Infrastructure as Code (IaC) is an important focus, allowing you to create and replicate collections, roles, indexes, and functions across different environments. Fauna Labs also has a number of templates and application skeletons that help you focus on features and deliver your applications quickly!

### Fauna Schema Migrate tool

The [Fauna Schema Migrate](https://github.com/fauna-labs/fauna-schema-migrate) (FSM) tool also allows you to setup and manage your Fauna resources as code. It provides support for schema migrations for larger teams, and shows how to use `Let()` statements to update your databases in a single transaction. You also can use FSM to deploy blueprints, adding common functionality to your Fauna database quickly and consistently.

![Fauna Schema Migrate screenshot](https://images.ctfassets.net/po4qc9xpmpuh/3lwdeB4cnJX5xKsdyvFTDD/bb63a1f6e60109f091c0336a45b53684/fauna-schema-migrate.png)

### Fauna Serverless Framework plugin

The [Fauna plugin](https://github.com/fauna-labs/serverless-fauna) for the [Serverless Framework](https://serverless.com) allows you to manage your databases and resources directly in your *serverless.yml* file. You can integrate it in your test and CI/CD pipeliness to keep your databases in sync across multiple environments. There's also an [example repository](https://github.com/fauna-labs/serverless-fauna-example) that demonstrates how to create, update, and delete collections, indexes, roles, and user-defined functions (UDFs).

![Serverless plugin deployment screenshot](https://images.ctfassets.net/po4qc9xpmpuh/1ytFRhzqmzBaAZHYCPG2I7/122b0fa649a6ec0bf50ada3717c2dbb0/serverless-fauna.png)

### Blueprints

[Fauna blueprints](https://github.com/fauna-labs/fauna-blueprints) are packages of resources defined in pure FQL that can be loaded using the Fauna Schema Migrate. You can load blueprints into your database to perform common tasks like [email verification](https://github.com/fauna-labs/fauna-blueprints/tree/main/official/auth/email-verification), [password reset](https://github.com/fauna-labs/fauna-blueprints/tree/main/official/auth/password-reset), [rate limiting](https://github.com/fauna-labs/fauna-blueprints/tree/main/official/rate-limiting), and more.

![Screenshot showing nested official blueprints](https://images.ctfassets.net/po4qc9xpmpuh/6wqqZDnpvm2m2At6EVGMXF/9323a8d29e475a3699b606cdc55219d4/blueprints.png)

## Helpful examples

Reading the [docs](https://docs.fauna.com) is great, but sometimes you need more complete examples to help you understand a concept or get you unstuck. Fauna Labs has a number of examples, from our flagship Fwitter app to an example demonstrating how to use document streaming for real time updates. You'll also find the sample code from Fauna blog posts.

### Fwitter

[Fwitter](https://github.com/fauna-labs/fwitter) is a Twitter clone that demonstrates Fauna's features and functionality. It uses a frontend-only approach that accesses Fauna directly for data storage, authentication, and authorization. It demonstrates basic concepts, such as storing and retrieving data, as well as more advanced concepts like securing your data with user-defined functions (UDFs) and attribute-based access control (ABAC). For more information on Fwitter, see the repository or [this CSS-Tricks article](https://css-tricks.com/rethinking-twitter-as-a-serverless-app/).

![Fwitter screenshot](https://images.ctfassets.net/po4qc9xpmpuh/7CAt3vZBAV6Urn5rwfJHHF/2bc889fe0ff3388368556784b2960f52/fwitter.png)

### Fauna authentication skeleton with Auth0

This [application skeleton](https://github.com/fauna-labs/faunadb-auth-skeleton-with-auth0) gives you a basic React app with a login flow using Auth0. The app creates an [AccessProvider](https://docs.fauna.com/fauna/current/security/external/access_provider.html) and configures your Fauna database to accept JWT tokens from Auth0 for authentication. With Auth0 and Fauna, you can implement [social login](https://auth0.com/learn/social-login), allowing users to login using providers like Twitter or Google and reducing signup friction.

### Streaming example

[This project](https://github.com/fauna-labs/fauna-streaming-example) is an example project that demonstrates Fauna's document streaming features. It's a React app that retrieves a page of references from a collection and opens streams on the documents that are currently present on the screen. When those documents are updated, it displays the new versions in real time.

![Screen capture of dynamically updating products](https://images.ctfassets.net/po4qc9xpmpuh/tuPs36xXcK4EbOhtDNipI/5cb34da0edf4e986108fe71b15f08464/streaming.gif)

## Community contributions

We created Fauna Labs for our developer community, but we also want to hear your voice and highlight your contributions. That's why we've enabled [GitHub discussions](https://docs.github.com/en/discussions) and connected [GitHub issues](https://docs.github.com/en/issues) to our internal tracking tool. We also welcome your contributions, from pull requests on existing code to new blueprints and even [transferring repositories](https://docs.github.com/en/github/administering-a-repository/managing-repository-settings/transferring-a-repository) that you think others will find useful!

## What comes next?

See a tool that you'd like to see officially supported? Create an issue and let us know! If there's a specific tool, template, or example that you would like to see, let us know with a [feature request](https://forums.fauna.com/c/feature-requests/2) on the [Fauna community forums](https://forums.fauna.com).

We are currently developing self-paced workshops to help you and your team build more effectively with Fauna. Check back regularly for this and other updates.

Not sure where to start? Explore the [Fauna Labs repositories](https://github.com/fauna-labs), or clone the [Fwitter app](https://github.com/fauna-labs/fwitter) and start building with Fauna today!
