# Eulerian Analytics Tracking

## Description

This Google Tag Manager Community template is available for the Eulerian Analytics attribution & data activation solution provided by Eulerian Technologies SAS (https://eulerian.com)

## Getting Started

* Register through an account representative at https://eulerian.com
* Add a new subdomain on your DNS Provider following our instructions (recommended)
* The Eulerian Analytics tag template allow you to install up to 3 different tags:

### Page view
This call is trigered during web page loading or following specific actions. Use this tag to measure metrics associated to visitor's navigation on your website like : number of visits, bounce rate, time spent on site...

You might want to exclude pages which should not be tracked when using the All Pages trigger (product pages and transaction confirmation page).

### Product page View
Collect your product data and measure your product pages visits.

You can exclude the page view tag triggering on your product pages in order to avoid counting twice page views.

### Cart Interaction
Measure a new cart that lasts 30 minutes by default and includes an unlimited number of products. The product data can be updated (remove/add a line, modify quantity) within those 30 minutes. Each user interaction reset the cart lifespan.

It is recommended to trigger this tag on events like : add to cart, cart page view, or when modifying items.

Please note that you can use a cumulative mode if you need to push incrementally cart product details or deactivate this option directly from this GTM TemplatE.

### Transaction
Use this tag to collect and measure transactions happening on your website. This tag has to be triggered from the confirmation page.

You can exclude the page view tag triggering on your confirmation page in order to avoid counting twice page views.

#### Conversion ID
Use your own transaction ID system on Eulerian when flagging a new order. Be sure that this value is unique otherwise Eulerian won't count it.
By default, the platform is automatically generating a new transaction ID.

#### Transaction Amount
Measure and attribute your transactions' generated revenue. 
By default, each transaction has fixed value amount of 1.

#### Transaction Amount Currency
Set this option to automatically convert transactions happening in different currencies to your Eulerian.io's main currency. Specify the currency code you need to use (either a specific string or a custom variable)

### Lead Event
Use this tag to measure specific custom events happening on your website that you want to analyze with your attribution models.

You can exclude the page view tag triggering on your confirmation page in order to avoid counting twice page views.

#### Conversion ID
Use your own transaction ID system on Eulerian when flagging a new order. Be sure that this value is unique otherwise Eulerian won't count it.
By default, the platform is automatically generating a new transaction ID.

### Internal Search Results
Use to collect your interal search queries performed by your visitors. You can add as many search attributes you need depending on your search tool.

You can exclude the page view tag triggering on your confirmation page in order to avoid counting twice page views.

## Documentation of Custom Fields

### Eulerian Tracking Domain
Copy-paste your custom subdomain (e.g. 12345.mydomain.com) if you are installing Eulerian Analytics directly on your web domain. If not, please contact your account manager to pickup our 3rd Party domain.

### Web Page Attributes

#### Page Group
Associate the current page to a page category. This level of segmentation is then available in your reportings and can also be used for activation purposes (e.g. measure the number of visitors for a specific page category)

#### Rewrite your Page Paths
It is recommended to either use URL path or custom pagenames when tracking across multiple pages. Set the page path rewriting if you need to clean your website's url structure.

### Context-Flags
Segment your visitors according to what types of contents they have been exposed to on your website on a specific period of time. Context Flags are custom attributes containing information related to user navigation.

### CRM Parameters
Add additional information to a visitor using CRM parameters. Warning : crm parameters have to be first defined on Eulerian before to be available in reportings.

### User information
Follow how your visitors move forward within your custom engagement funnel. Each step of this funnel is called an engagement profile/
You can also collect different user identifiers within this tag like your user unique id (UID) to merge different devices into a single user profile.

### Advanced configuration
This section includes different options to deactivate page view counts, blocks connectors firing, or activate the debug mode to display information in your web console like the datalayer.