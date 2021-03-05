---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: Home
permalink: /
nav_order: 1
---

# Marketplacer API documentation

Marketplacer has 2 APIs available, the one you choose to develop with will be driven by the _use-cases_ that you are developing for - so choose wisely!

<br/>

![The GraphQL API is our marketplace-wide API, it allows greater access to data across that domain, including much of the data available via the V2 (REST) API. Some of the common use-cases for this API are: managing marketplace categorizations, developing your own Marketplacer front end and querying data across the marketplace.](/assets/images/graphql_banner.png)

[Get Started with GraphQL](http://example.com/){: .btn .btn-purple }

<hr>



![The V2 (REST) API is focused on the individual seller on the marketplace, (remember a marketplace can have many sellers). Some of the common use-cases for this API are: sellers retrieving their invoices, sellers automating advert creation and sellers setting stock levels for their adverts.](/assets/images/rest_banner.png)

[Get Started with V2 (REST)](http://example.com/){: .btn .btn-blue }

<hr>



We also provide access to Webhooks, which allow users to subscribe to real-time notifications from Marketplacer. Webhooks are available at both the marketplace and individual seller level.

![Webhooks allow clients to subscribe to notifications from Marketplacer, across a number of entities, avoiding the need to poll for updates.](/assets/images/webhooks_banner.png)

[Get Started with Webhooks](http://example.com/){: .btn}

---

### At a glance..

A summarised comparison of objects, queries, mutations and notifications for both APIs and webhooks can be found below.

**Note:** A “mutation” here, (nomenclature lifted from the world of GraphQL), refers either to a Create, Update or Delete operation – refer to the full documentation to see which of these operations are available for each API.

<br/>

![The GraphQL API can query sellers, adverts, variants, carts, orders, invoices, shipment and taxonomy. The GraphQL API can mutate carts, orders, invoices and taxonomy. The V2 (REST) API can query adverts, variants, invoices and shipments. The V2 (REST) API can mutate adverts, variants, invoices and shipments.](/assets/images/apicomparison.png)