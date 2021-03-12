---
layout: page
title: Advert
permalink: /restapi/endpoints/advert
nav_order: 1
parent: Endpoints
grand_parent: V2 (REST) API
---

# Advert

## What is an Advert?

When we say “Advert” in Marketplacer, we really mean a Product or Service that’s been placed for sale (by a Seller) on the Marketplace.

It’s that simple!

The reasoning behind this naming convention stems from the fact that we cater for the following types of Advert, (so the use of just “Product” would not suffice):

- Product
- Service
- Event
- Holiday

So again, for the purposes of reading the API documentation, when you see Advert, think **Product**…

### Adverts Vary

Products listed for sale on Marketplacer can of course vary, so think of the Advert as a pair of running shoes, and the _**Variants**_ as the Size and Colour combinations, e.g.:

- Black / Size 10
- White / Size 11

And so on…

We represent _**Variants**_ as a separate resource type in the API, see Variant Endpoint, but as we refer to them in our discussion of Adverts it’s worth mentioning them here.

<hr>

## Get All Adverts

This endpoint will return a paginated collection of your adverts, as well as their associated brands and taxons.

### Request

```shell
GET /api/v2/client/adverts
```

<br>
You can filter by `external_id` to return only adverts with that `external_id`.

    GET /api/v2/client/adverts?external_id=VALUE

<br>
You can also filter to only return adverts whose variants have a particular value for the `sku` or `barcode`.

    GET /api/v2/client/adverts?sku=VALUE

### Response

<%= headers 200 %>
<%= collection [advert], included: [taxon, brand], pagination: "/api/v2/client/adverts" %>

<hr>

## Get an Individual Advert

<hr>

## Creating an Advert

<hr>

## Updating an Advert

<hr>

## Deleting an Advert
