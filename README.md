
# Netlife Technical Strategy

![Alt tech stack](tech_stack_with_logos.png?raw=true "Tech stack")

## Introduction

This is a guideline describing the technical strategy of Netlife Design AS moving forward from 2019 into the future. It aims at suggesting a stable and standardized path for all new projects in order to structure the way we work and improve our efficiency, our flexibility, our quality, our ability to maintain and the expertise we offer.

***

## Netlife tech strategy - principles

1. We develop open source code and share whatever we can
2. We follow the principles in the JAMstack, separating the frontend from the backend
3. Our frontend applications are user oriented, written using the React framework
4. We use headless CMS's solutions when we can (preferably Sanity, Craft or Enonic)
5. Technical partners have 100% responsibility for the backend if any exist
6. If other frontend technologies is pre-determined we deliver design or HTML/CSS/JS

***

### Fixing the world one step at a time

Netlife believe in taking small steps for a better world. A consequence of the strategy is decoupling systems. What that really means is separating the different parts into individual components. We make it cheaper and simpler for our customers to replace one part of their solution. To replace us...

Netlife does not want to create lock-in situations where customers cannot afford to make the right decisions. We should deserve our customers. We want customers to turn to us because they want to improve or solve problems. We want to enable a fair world where we have to prove ourselves worthy to keep customers trust over time.

### Stakeholders

In any strategy there are considerations which limits the freedom and deciding power we can allow ourselves. There are areas which tech control fully and holly where we can, and should, own the domain and all the decisions within it. There are other areas where we share the domain with other stakeholders, and we need to share decisions. And lastly there are domains where we clearly do not own the domain, even if we work within it, and can only influence or suggest certain strategic goals. We need to be considerate to the people we work with, and respect that there are several sides to any coin.

### Outliers and Exceptions

A strategy can never be a perfect fit for every solution. Constraints and requirements can overrule a strategy where there is good cause. For this reason the rules and guidelines provided in this document needs to be general enough to support common use cases, open enough to inspire creativity and concrete enough to be of value.

The most typical scenario where the strategy does not align well with the requirement is a heavy content driven project where the customer want to be able to make major changes to the templates/view and/or control where content-blocks are placed in the view. Identifying and challenging this would be key to see if the suggested architecture and strategy is the best fit or not.

### Evolution

Nothing lasts. Similar to code and documentation a strategy begins to deteriorate as soon as its written. Everything will eventually change. Therefore there will never be a _final_ version of this strategy, there will be only a current one waiting to be improved in order to fit the larger and current picture of the world as it might be.

As such it encourages everyone to opinionate, improve and suggest changes to this document. It's not supposed to be owned by one single entity, it is by nature a shared commodity in which we all align to and, as far as possible, agree on.

### Time is on our side

Rome was not built in a day. A strategy cannot be expected to be fruitful immediately. We must iteratively and slowly transition wherever we can. Our motivation should be to getting a small step closer every single day. But tech cannot do it alone as we are not separate from the rest of Netlife. We need the entire organisation to believe what we believe, our partners to align with our guidelines and hope to convince new and existing customers to embrace the brand new world.

***

## The dawn of opportunity

There exists movements in the community which align well with the direction we are leaning internally. We are struggling with a certain set of repetative challenges like handovers, partners and missmatch between design and implementation. Aligning with the general directions and decisions proposed in this strategy would alleviate some of that pain, but needs to be done in a considerate and respectful manner to those afflicted by them.

### Headless is the future

Autonomy-, decoupling-, RESTful-, microservice-, DomainDrivenDesign- and abandonment of monolithic architecture- trends has been growing for quite a while, decoupling web applications (presentation separated from the backend) follows that same pattern. The maturing of SPA applications, Node/npm, GitHub, SEO requirements, SaaS cloud models and enriched tooling enable a new direction.

Headless options for new and existing CMS platforms are ***game changing***. There are technical improvements which certainly can improve development experiences and delivery quality, however these are _minor_ improvements compared to what headless offers to the table. And the list of platforms that are taking the headless approach is constantly growing ([headlesscms.org](https://headlesscms.org/)).

### The JAMstack

![The JAMstack](jamstack_logo.png?raw=true "The JAMstack")

One cannot for certain confirm that the term [JAMstack](https://jamstack.org/) originated from Mathias Biilmann at [Netlify](https://netlify.com), but one can trace most of its push back to Netlify at least.

What the [JAMstack (wtf?)](https://jamstack.wtf) propose is a high focus on the front end builds, eluding server-side functions as much as possible. The three major elements are:

#### J - Javascript

Javascript on the client-side handling communication requests and responses. Although not limited to, front-end SPA frameworks like [React](https://reactjs.org) fits this model well.

#### A - APIs

Server-side processes, including database handling, are accessed by JS-driven [HTTP(s)](https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol) calls. JAMstack is by default API and technology agnostic, communicating with all external sources over HTTP, caring about the data and structure only.

#### M - Markup

This term Markup again relate to an agnostic attitude towards creating or rendering sites users can actually see. This declaratively suggests using build tools and encourage the use of static site generator techniques.

### The MVC pattern

One can argue wheather a true MVC [(Model-view-controller)](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller) pattern can be achieved in web development, but the concepts of separating database logic (M), presentation logic (V) and application logic (c) are neatly built into how most web framework best-practice examples are structured.

### Completing the deploy circle

Following the JAMstack path would as such enable the use of [CDNs](https://en.wikipedia.org/wiki/Content_delivery_network) (or [ADNs](https://en.wikipedia.org/wiki/Application_delivery_network)) hosting of static applications fully [SEO](https://en.wikipedia.org/wiki/Search_engine_optimization) optimized with high-availability and performance. [Git](https://en.wikipedia.org/wiki/Git)-centric continuous deployment strategies through pushing changes. And it reduces security concerns greatly with removing the attack vectors of traditionally coupled systems (it does not remove it completely mind you). The proposed architecture would also fit in nicely with serverless [BaaS](https://en.wikipedia.org/wiki/Mobile_backend_as_a_service) function paradigms.

## Pro's and con's

Every shift in direction come with benefits and disadvantages. It is important to understand and know about what these are so that we may face the consequences well prepared and in agreement. Hence the following sections outline how different areas are affected in a more direct manner. The benefits ***are*** greater than the drawbacks in a heuristic perspective, which is why the chapters are positively named.

### Netlife strategy

The overall Netlife strategy aims at moving towards delivering more product and service oriented solutions. What that means is delivering more data-oriented applications as a supplement to our historically strong content-oriented application projects. The consequences of this could be to deliver web-applications with a whole range of different backends, including custom developed backends. Today most of our projects are content driven, often powered by a [CMS](https://en.wikipedia.org/wiki/Content_management_system). The strategy suggests a supplementary shift in that focus.

What service/product systems have in common is that they are highly interactive, are feature driven and where the datamodel and structure is often inherited from, or dependent on, external or existing systems. These schenarios typically have a separated frontend and backend. A great way to gain experience for coming projects would be to use these kinds of structures and architectures in areas with less risk. The proposed technical strategy aligns with our wanted market position and projects, proposed in our Netlife strategy.

### Customer benefits

There are disadvantages on the customer side. One is an increased setup cost for full stack applications which includes both a frontend and a backend. In a JAMstack architecture most customers without technical inhouse resources would find making big changes to templates or the presentation of content more difficult without expert help. Content and text by itself should not be a problem, but the ability to add a new page template and present that on their website is not done purely from the CMS, which is a disadvantage for semi advanced users.

It might even be the case that two separate solutions could possibly be delivered from two different companies. Contracts and formal support structures may have to be redefined or improved.

Benefits worth mentioning would be licensing and price. Most of the ecosystem (depending on platform of choice) offer very reasonable pricing models for quite extensive tooling and tech setup. It includes none of the drawbacks some architectures and stacks have on SEO. It enables a customer to choose, and replace, the frontend and backend seperately. Arguably the cost of an eventual migration will be significantly lower and easier to manage (or contain rather).

Due to separation of concern, it is safe to assume that once in place the JAMstack architecture will be a cheap and reliable solution. However, existing or already implemented CMS platforms could challenge, and even prevent, the optimal architecture for a given set of customers. There are legacy systems out there (we have even created many), and we need to transition slowly, if at all, depending on the customer. Hybrid solutions may be good alternatives to combine the best of both worlds.

### Partner benefits

A clear separation between the frontend and backend should make it easier to identify responsibility. Estimation and status for separate deliveries should also easier to understand and report on as the exchange currency is data, through defined endpoints. Is should improve collaboration and mandate in a more concise way than previously.

The most important beneficial effect however would be ownership and simplicity. No longer should uncertainty of handover and re-implementation of functional prototypes be an issue. Either Netlife deliver prototypes (typically in Figma or HTML) or the full frontend application.

The most important drawback would be that one side of a messy partnership needs to let go of a part of the solution, in other words release control of some of the revenue stream. If the parties are working in collaboration on the frontend, one side needs to let the other handle all of it or none of it.

### Internal benefits

Not everyone is as comfortable with this way of developing applications. A starting hurdle is to be expected as previous development styles, or habit. There will be a defining change in how we utilize a CMS, and how we would work in a scenario where we deliver both the backend and frontend. Some people may be exteremely skilled in how to setup a project in a spesific CMS and might now have to reinvent the most efficient way set up projects.

We would be required to work the same way, through the same architecture and the same methodology regardless of which parts of the stack we take responsibility for delivering.

#### Clearly defined delivery expectations

Netlife will deliver the entire frontend of a solution, HTML/CSS prototypes or nothing at all. Gone are the days of developing an application which in the end is torn apart, cut to pieces and reimplemented into any given CMS templating engine. There should be no double implemenentation costs.

It will also be simpler to define and explain which CMS we could develop and configure internally, which we would always use a partner for the backend and which we won't support at all.

#### Flexibility

We will all be working on the same set of frontend technologies therefore the steep learning curve to understand and master every CMS specific templating engines would be greatly reduced. We should be highly effective and flexible in moving from one solution to the next in our roles as frontend developers.

#### Specialized experts

When working with a defined subset of technologies and a set architecture we would specialize in them to a greater extent. It would also be natural to believe that fractions would form in terms of pure frontend, fullstack or CMS/backend developers would emerge. Some would want to be involved in several of these groups, some in perhaps only one of them which would ultimately help us becoming even more specialized. It opens a door where we increasingly would be able to share and contribute to the ecosystem. It might even prove to give us a unique standing in the technical community or if nothing else aquire high confidence and experience in what we are doing. Becoming masters of the art so to speak.

#### Talent, training, onBoarding and recruitment

Another benefit would be simplicity in finding new talent in certain technologies. The cost and time of training and onboarding would be reduced, and new people would be able to create value earlier than before since the landscape one needs to master is smaller and more defined. The actual recruitment process would also be more direct and concise as we know exactly what kind of talent we are looking for, and provide transparent information of the technologies we are working with.

#### Lifecycles, quality, hosting and maintainance

The amount of **stuff** we need to maintain and know decreases significantly because the sum of variations decrease over time. We can also streamline the tools and functions required to monitor, surveil and ensure high availability. It enables ***"one"*** standard way of deployment and a standard way to handle persistance.

Another benefit would be on the side of testing. Even if we can allow a multiture of tools to perform testing, the separation of front/back-end would standarize the way we test communication and build integrations.

### Adaptability and evolution

Even if the strategy propose a clear path moving forward, there should be plenty of room to explore and innovate. The proposed strategy focuses mainly on a direction and does not eliminate new paths or future expansion of technology in the future. The industry evolve and changes daily, and we need to keep up. As our strategy must evolve as must our technical solutions.

### Wrapup

Betting on a future of headless CMS, JAMstack architecture and high performing applications would long term put Netlife firmly on the map as technologists. Even if vendors, platforms and technologies go out of favor, we would be better able to adapt in an unknown future.

In the end we enable a more fair world where we have to prove ourselves worthy to keep the trust of our customers. And there is nothing in our technical strategy which does not align closely with the overlying Netlife strategy.

***

## Domains, ownership and evaluations

This section covers a more detailed look into some important domains to shed some light into spesific handling of these evaluating many stakeholders and perspectives.

### CMS

As far as the customer goes, Netlife should be seen as a platform independent partner.

The domain of CMS does not really belong to tech. The choice of CMS platform should not be based on technical preference, although it most certainly should depend on technical requirements which can direct the choice. All CMS platforms have strengths and weaknesses. Some waknesses are too big, or so far from our strategy, that they are ruled out. But in the end the choice should be made based on the requirement of the administering users of our customer and the features we need to support.

Refusing to work with a certain CMS platform if the architecture aligns with our strategy, is simply put a folly on our part. We should not, and cannot dictate this choice, but we should provide honest and well meaning advice. There is just too much opportunity at stake, in a demanding market, to turn our back based on technical preference.

That is not to say we are to say yes to deliver anything on any platform, but we should be able to provide our customers excellent frontend web applications whenever we can, unless we explicitly have chosen not to.

***

### Design and CSS

This is a domain we share with others. As technologists we are merely translators of design, and we need to establish how to collaborate with others to achieve the best result should work. We want others to contribute with their expertise as efficiently as possible. We aim at being an extension of their work and complement others strengths.

Hence the technologies, frameworks and tools we utilize needs to consider collaboration. The same goes for choices of implementation style. We can suggest improvements and tools, and if successful we will sufficiently train and help others to be as efficient as possible when conducting their job, just as we would expect them to view our challenges and efforts.

***

## Resources of interest on the internetz

- [General](#general)
- [Platforms](#platforms)
- [JAMstack Sites Showcase](#jamstack-sites-showcase)
- [Static Site Generators](#static-site-generators)
- [CMS](#cms)
- [API](#api)
  - [Authentication](#authentication)
  - [Comments](#comments)
  - [Forms](#forms)
  - [E-commerce](#e-commerce)
  - [Search](#search)
  - [Database](#database)
- [Serverless](#serverless)
- [Videos](#videos)
- [Tutorials / Articles](#tutorials--articles)
- [Podcasts](#podcasts)

***---***

## General

- [JAMstack](https://jamstack.org/)
- [JAMstack resources](https://jamstack.org/resources/) - Videos and articles about JAMstack.
- [the New Dynamic](https://www.thenewdynamic.org/) - Frikking awesome library of examples, tools and services.

## Platforms

- [GitHub Pages](https://pages.github.com/) - Website hosting from your GitHub repo.
- [Netlify](https://netlify.com) - All-in-one platform for automating modern web projects.
- [ZEIT Now](https://zeit.co) - All-in-one serverless platform for modern web apps with config-free tools and workflows.

## JAMstack Sites Showcase

- [React](https://reactjs.org/) - Built on Gatsby.
- [Squoosh.app](https://squoosh.app/) - Hosted on Netlify, demonstrates advanced features from a modern Web Application.
- [Hopper](https://travel.hopper.com/) - Built on Gatsby and hosted on Netlify.
- [VSCode Power User Course](https://vscode.pro/) - PWA built on Gatsby and hosted on Netlify.
- [CloudyCam](https://CloudyCam.dev/) - PWA built on Next.js and hosted on Zeit Now v2 Serverless platform.

## Static Site Generators

- [Gatsby](https://gatsbyjs.org) - Blazing-fast static site generator for React.
- [Next.js](https://nextjs.org/) - Lightweight framework for static and server-rendered applications.
- [Metalsmith](https://metalsmith.io) - An extremely simple, pluggable static site generator.
- [eleventy](https://www.11ty.io/) - A simpler static site generator transforming various template files into HTML.

*For a more complete list see [StaticGen](https://www.staticgen.com/).*

## Headless CMS documentation

- [Contentful](https://contentful.com) - Content infrastructure for digital teams.
- [NetlifyCMS](https://netlifycms.org/) - open source Git-based CMS.
- [Sanity](https://www.sanity.io/) - Headless CMS and Content API.

- [Headless Craft CMS](https://craftquest.io/courses/headless-craft) - Element API and CraftQL alternatives introduction.

- [Headless Enonic XP](https://enonic.com/developer-tour/headless-cms) - Graphql powered CMS API with Enonic.

- [Headlesss Hybrid Episerver CMS](https://www.episerver.no/produkter/funksjoner/alle-funksjoner/headless-api/) - headless decoupled CMS backend for frontend web development in Episerver.

### Authentication

- [Auth0](https://auth0.com/) - Single sign on and token based authentication.
- [Netlify Identity](https://www.netlify.com/docs/identity/) - Brings a full suite of authentication functionality

### Comments

- [Disqus](https://disqus.com) - Global comment system that improves discussion on websites and connects conversations across the web.
- [Facebook Comments](https://developers.facebook.com/docs/plugins/comments) - The comments plugin lets people comment on content on your site using their Facebook account.
- [Utterances](https://utteranc.es/) - A lightweight comments widget built on GitHub issues. Use GitHub issues for blog comments, wiki pages and more.

### Forms

- [Netlify Forms](https://www.netlify.com/docs/form-handling/) - Built-in form handling on building time by parsing HTML files directly at deploy time.

### E-commerce

- [Flatmarket](https://github.com/christophercliff/flatmarket) - Flatmarket is a free, open source e-commerce platform for static websites.
- [GoCommerce](https://www.gocommerceapi.org) - A headless e-commerce for JAMstack sites.
- [Snipcart](https://snipcart.com/) - A powerful shopping cart platform for developers.
- [Moltin](https://moltin.com/) - eCommerce API for developers.
- [Trolley](https://trolley.link) - A shopping cart designed for the JAMstack.

### Search

- [Algolia](https://www.algolia.com/) - The most reliable platform for building search into your business.
- [Lunr](https://lunrjs.com/) - Search made simple (on frontend).
- [CloudSh](https://cloudsh.com/) - Powerful search with a few lines of JavaScript.

### Database

- [GraphQL](https://graphql.org) - Query language for APIs and a runtime for fulfilling those queries with your existing data.
- [MongoDB](https://www.mongodb.com/) - Document-based distributed database for the cloud.
- [Elastic](https://www.elastic.co/) - The ELK stack for infinite searching at scale.

## Serverless

- [Netlify Functions](https://www.netlify.com/docs/functions/) - Netlify lets you deploy Lambda functions without an AWS account, and with function management handled directly within Netlify.
- [Amazon Lambda](https://aws.amazon.com/lambda/) - Lets you run code without provisioning or managing servers.
- Microsoft Azure
  - [Azure Functions](https://docs.microsoft.com/en-us/azure/azure-functions/) - Serverless compute service that enables you to run code on-demand without having to explicitly provision or manage infrastructure.
  - [Azure Logic Apps](https://docs.microsoft.com/en-us/azure/logic-apps/) - Simplifies building automated scalable workflows that integrate apps and data across cloud services and on-premises systems.
- Google Cloud
  - [App Engine](https://cloud.google.com/appengine/) - Serverless application that completely abstracts away infrastructure so you focus only on code.
  - [Cloud Functions](https://cloud.google.com/functions/) - Serverless environment to build and connect cloud services.
  - [Cloud Datastore](https://cloud.google.com/datastore/) - Highly-scalable NoSQL database with automatic sharding and replication.
  - [Cloud Storage](https://cloud.google.com/storage/) - Geo-redundant object storage for high QPS needs.
  - [Cloud Pub/Sub](https://cloud.google.com/pubsub/) - Geo-redundant real-time messaging for all message sizes and velocities.
  - [Apigee](https://apigee.com/) - Enterprise API management for multi-cloud environments.
  - [Endpoints](https://cloud.google.com/endpoints/) - API management apps built on Google Cloud.
  - [Cloud Dataflow](https://cloud.google.com/dataflow/) - Serverless stream and batch data processing service.
  - [BigQuery](https://cloud.google.com/bigquery/) - Serverless data warehousing services that help you to deploy advanced cloud data warehousing solutions for your enterprise.
  - [Cloud ML Engine](https://cloud.google.com/ml-engine/) - Serverless machine learning services that automatically scales built on custom Google hardware (Tensor Processing Units).
- [Serverless](https://serverless.com/) - Toolkit for deploying and operating serverless architectures.
- [Cloudinary](https://cloudinary.com/) - Serverless media (images/videos) management platform. Provides SDKs in every popular language and media widgets for JAMstack to make it easy to manage media, CDN, storage, transformations, and more.

*For a more complete list see [Awesome Serverless](https://github.com/pmuens/awesome-serverless).*

## Videos

- [The New Front-end Stack. JavaScript, APIs and Markup](https://vimeo.com/163522126) - Matt Biilmann.
- [Rise of the JAMstack](https://www.youtube.com/watch?v=uWTMEDEPw8c) - Mathias Biillman.

- [Git-based or API-driven CMS](https://www.youtube.com/watch?v=KX4G49ZrvY0) - Chris Macrae.
- [JAMstack Tutorial - Full site using Netlify & Hugo](https://www.youtube.com/watch?v=NSts93C9UeE) - freeCodeCamp.org.
- [Gatsby JS Crash Course](https://www.youtube.com/watch?v=6YhqQ2ZW1sc) - Traversy Media.
- [How We Got Here and The Future of the Web](https://www.gatsbyjs.com/gatsby-days-keynote-kyle/) - Kyle Mathews.

## Tutorials / Articles

- [Ghost on the JAMstack](https://blog.ghost.org/jamstack/)
- [Getting Started with Gatsby and Cockpit — Part 1 of 2](https://blog.ginetta.net/getting-started-with-gatsby-and-cockpit-part-1-of-2-d86871932d44)
- [Creating Static E-commerce site with GatsbyJs](https://medium.com/@pinku1/creating-static-e-commerce-site-with-gatsbyjs-a349d7e022a)
- [For Static Sites, There’s No Excuse Not to Use a CDN](https://forestry.io/blog/for-static-sites-theres-no-excuse-not-to-use-a-cdn/)
- [E-commerce front-end for Vue.js, Nuxt.js and Snipcart](https://www.sanity.io/blog/e-commerce-vue-nuxt-snipcart)
- [Building Paul The Octopus](https://www.tomango.co.uk/thinks/paul-the-octopus-2018/)
- [JAMstack and Netlify: Do We really need another buzzword?](https://noti.st/philhawksworth/qp7jZC/jamstack-and-netlify-do-we-really-need-another-buzzword)
- [The JAMstack Startup Landscape](https://medium.com/@CRVVC/the-jamstack-startup-landscape-c06cc3cdb917)
- [How I built my blog using Gatsby and Netlify](https://blog.pavsidhu.com/how-i-built-my-blog-using-gatsby-and-netlify/)
- [Developer's Guide to Headless E-Commerce](https://snipcart.com/blog/headless-ecommerce-guide)
- [Handling Static Forms, Auth & Serverless Functions with Gatsby on Netlify](https://snipcart.com/blog/static-forms-serverless-gatsby-netlify)
- [JAMstack for Clients: Benefits, Static Site CMS, & Limitations](https://snipcart.com/blog/jamstack-clients-static-site-cms)
- [Exploring Netlify CMS, a React & Git-Based Content Management System](https://snipcart.com/blog/netlify-cms-react-git-workflow)
- [JAMstack PWA — Let’s Build a Polling App. with Gatsby.js, Firebase, and Styled-components Pt. 1](https://medium.com/@UnicornAgency/jamstack-pwa-lets-build-a-polling-app-with-gatsby-js-firebase-and-styled-components-pt-1-78a03a633092)
- [Dynamic Static Sites with Netlify and iOS Shortcuts; Use Netlify Functions, a Gulp build process and iOS Shortcuts to publish dynamic content to your static site](https://bryanlrobinson.com/blog/2018/11/12/ios-shortcuts-pushing-data-to-netlify-static-site/)
- [Gatsby for Apps](https://www.gatsbyjs.org/blog/2018-11-07-gatsby-for-apps/)
- [Turning the Static Dynamic](https://www.gatsbyjs.org/blog/2018-12-17-turning-the-static-dynamic/)
- [Going JAMstack with Netlify and Nuxt](https://blog.lichter.io/posts/going-jamstack-with-netlify-and-nuxt/)
- [Getting Started With Gridsome](https://scotch.io/tutorials/getting-started-with-gridsome)
- [The Complete Beginner's Guide to Deploying Your First Static Website to IPFS](https://interplanetarygatsby.com/ipfs-deploy/)
- [A Broad Discussion on JAMstack & E-Commerce (Podcast & Transcript)](https://snipcart.com/jamstack-ecommerce-podcast)

## Podcasts

- [JAMstack Radio](https://www.netlify.com/tags/podcast/)

### Lastly

**Shoutout to Vilson Vieira (automata)** for an awesome resource collection

***
