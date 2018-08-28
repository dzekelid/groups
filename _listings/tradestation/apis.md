---
name: TradeStation
x-slug: tradestation
description: Whether you trade stocks, ETFs, options or futures, TradeStation???s
  award-winning tools and brokerage services can give you the confidence to achieve
  your goals.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tradestation_logo_285x40.png
x-kinRank: "7"
x-alexaRank: "37688"
tags: Groups
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/tradestation/apis.md
specificationVersion: "0.14"
apis:
- name: Tradestation API - Confirm Group Order
  x-api-slug: ordersgroupsconfirm-post
  description: |-
    Returns estimated cost and commission information for a group of orders (OCO, BRK) without the orders actually being placed

    **Base Confirmation**  (All confirmations will have these fields)
    * Route
    * Duration
    * Account
    * SummaryMessage
    * OrderConfirmId

    **Equity Confirmation** (Base Confirmation fields + the following)
    * EstimatedPrice
    * EstimatedPriceDisplay
    * EstimatedCost
    * EstimatedCostDisplay
    * EstimatedCommission
    * EstimatedCommissionDisplay

    **Forex Confirmation** (Base Confirmation fields + the following)
    * BaseCurrency
    * CounterCurrency
    * InitialMarginDisplay

    **Futures Confirmation** (Base Confirmation fields + the following)
    * ProductCurrency
    * AccountCurrency
    * EstimatedCost
    * EstimatedPrice
    * EstimatedPriceDisplay
    * InitialMarginDisplay
    * EstimatedCommission
    * EstimatedCommissionDisplay
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tradestation_logo_285x40.png
  humanURL: http://www.tradestation.com
  baseURL: https://api.tradestation.com//v2
  tags: Technology, Financial Services, Financial, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/tradestation/ordersgroupsconfirm-post-openapi.md
- name: Tradestation API - Submit Group Order
  x-api-slug: ordersgroups-post
  description: "Submits a group order such as Bracket and OCO Orders.\n\n#### Order
    Cancels Order (OCO)\nAn OCO order is a group of orders whereby if one of the orders
    is filled\nor partially-filled, then all of the other orders in the group are\ncancelled.\n\n####
    Bracket OCO Orders\nA bracket order is a special instance of an OCO (Order Cancel
    Order).\nBracket orders are used to exit an existing position. They are designed\nto
    limit loss and lock in profit by ???bracketing??? an order with a\nsimultaneous
    stop and limit order.\n\nBracket orders are limited so that the orders are all
    for the same\nsymbol and are on the same side of the market (either all to sell
    or\nall to cover), and they are restricted to closing transactions.\n\nThe reason
    that they follow these rules is because the orders need to be\nable to auto decrement
    when a partial fill occurs with one of the orders.\nFor example, if the customer
    has a sell limit order for 1000 shares and\na sell stop order for 1000 shares,
    and the limit order is partially\nfilled for 500 shares, then the customer would
    want the stop to remain\nopen, but it should automatically decrement the order
    to 500 shares to\nmatch the remaining open position.\n\n### Errors\nWhen a submitted
    order fails, it can be seen in two different ways:\n-\tImmediately rejected during
    submit to the Orders API with a 400 HTTP status code.\n-\tAccepted by the API
    with a 200 HTTP status code, but you will see the order with a status of ???REJ???
    (rejected) when you fetch the Order from the /v2/accounts/{id}/orders API\n\n####
    NOTE\nWhen a group order is submitted, the order execution system treats each
    sibling order as an individual order. Thus, the system does not validate that
    each order has the same Quantity, and currently it is not able to update a bracket
    order as one transaction, instead you must update each order within a bracket.\n\nIn
    order to prevent errors, please validate the data on the client side."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tradestation_logo_285x40.png
  humanURL: http://www.tradestation.com
  baseURL: https://api.tradestation.com//v2
  tags: Technology, Financial Services, Financial, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/tradestation/ordersgroups-post-openapi.md
- name: Tradestation API - Submit Group Order
  x-api-slug: ordersgroups-post
  description: "Submits a group order such as Bracket and OCO Orders.\n\n#### Order
    Cancels Order (OCO)\nAn OCO order is a group of orders whereby if one of the orders
    is filled\nor partially-filled, then all of the other orders in the group are\ncancelled.\n\n####
    Bracket OCO Orders\nA bracket order is a special instance of an OCO (Order Cancel
    Order).\nBracket orders are used to exit an existing position. They are designed\nto
    limit loss and lock in profit by ???bracketing??? an order with a\nsimultaneous
    stop and limit order.\n\nBracket orders are limited so that the orders are all
    for the same\nsymbol and are on the same side of the market (either all to sell
    or\nall to cover), and they are restricted to closing transactions.\n\nThe reason
    that they follow these rules is because the orders need to be\nable to auto decrement
    when a partial fill occurs with one of the orders.\nFor example, if the customer
    has a sell limit order for 1000 shares and\na sell stop order for 1000 shares,
    and the limit order is partially\nfilled for 500 shares, then the customer would
    want the stop to remain\nopen, but it should automatically decrement the order
    to 500 shares to\nmatch the remaining open position.\n\n### Errors\nWhen a submitted
    order fails, it can be seen in two different ways:\n-\tImmediately rejected during
    submit to the Orders API with a 400 HTTP status code.\n-\tAccepted by the API
    with a 200 HTTP status code, but you will see the order with a status of ???REJ???
    (rejected) when you fetch the Order from the /v2/accounts/{id}/orders API\n\n####
    NOTE\nWhen a group order is submitted, the order execution system treats each
    sibling order as an individual order. Thus, the system does not validate that
    each order has the same Quantity, and currently it is not able to update a bracket
    order as one transaction, instead you must update each order within a bracket.\n\nIn
    order to prevent errors, please validate the data on the client side."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tradestation_logo_285x40.png
  humanURL: http://www.tradestation.com
  baseURL: https://api.tradestation.com//v2
  tags: Technology, Financial Services, Financial, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/tradestation/ordersgroups-post-openapi.md
- name: Tradestation API - Submit Group Order
  x-api-slug: ordersgroups-post
  description: "Submits a group order such as Bracket and OCO Orders.\n\n#### Order
    Cancels Order (OCO)\nAn OCO order is a group of orders whereby if one of the orders
    is filled\nor partially-filled, then all of the other orders in the group are\ncancelled.\n\n####
    Bracket OCO Orders\nA bracket order is a special instance of an OCO (Order Cancel
    Order).\nBracket orders are used to exit an existing position. They are designed\nto
    limit loss and lock in profit by ???bracketing??? an order with a\nsimultaneous
    stop and limit order.\n\nBracket orders are limited so that the orders are all
    for the same\nsymbol and are on the same side of the market (either all to sell
    or\nall to cover), and they are restricted to closing transactions.\n\nThe reason
    that they follow these rules is because the orders need to be\nable to auto decrement
    when a partial fill occurs with one of the orders.\nFor example, if the customer
    has a sell limit order for 1000 shares and\na sell stop order for 1000 shares,
    and the limit order is partially\nfilled for 500 shares, then the customer would
    want the stop to remain\nopen, but it should automatically decrement the order
    to 500 shares to\nmatch the remaining open position.\n\n### Errors\nWhen a submitted
    order fails, it can be seen in two different ways:\n-\tImmediately rejected during
    submit to the Orders API with a 400 HTTP status code.\n-\tAccepted by the API
    with a 200 HTTP status code, but you will see the order with a status of ???REJ???
    (rejected) when you fetch the Order from the /v2/accounts/{id}/orders API\n\n####
    NOTE\nWhen a group order is submitted, the order execution system treats each
    sibling order as an individual order. Thus, the system does not validate that
    each order has the same Quantity, and currently it is not able to update a bracket
    order as one transaction, instead you must update each order within a bracket.\n\nIn
    order to prevent errors, please validate the data on the client side."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tradestation_logo_285x40.png
  humanURL: http://www.tradestation.com
  baseURL: https://api.tradestation.com//v2
  tags: Technology, Financial Services, Financial, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/tradestation/ordersgroups-post-openapi.md
- name: Tradestation API - Confirm Group Order
  x-api-slug: ordersgroupsconfirm-post
  description: |-
    Returns estimated cost and commission information for a group of orders (OCO, BRK) without the orders actually being placed

    **Base Confirmation**  (All confirmations will have these fields)
    * Route
    * Duration
    * Account
    * SummaryMessage
    * OrderConfirmId

    **Equity Confirmation** (Base Confirmation fields + the following)
    * EstimatedPrice
    * EstimatedPriceDisplay
    * EstimatedCost
    * EstimatedCostDisplay
    * EstimatedCommission
    * EstimatedCommissionDisplay

    **Forex Confirmation** (Base Confirmation fields + the following)
    * BaseCurrency
    * CounterCurrency
    * InitialMarginDisplay

    **Futures Confirmation** (Base Confirmation fields + the following)
    * ProductCurrency
    * AccountCurrency
    * EstimatedCost
    * EstimatedPrice
    * EstimatedPriceDisplay
    * InitialMarginDisplay
    * EstimatedCommission
    * EstimatedCommissionDisplay
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tradestation_logo_285x40.png
  humanURL: http://www.tradestation.com
  baseURL: https://api.tradestation.com//v2
  tags: Technology, Financial Services, Financial, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/tradestation/ordersgroupsconfirm-post-openapi.md
- name: Tradestation API - Confirm Group Order
  x-api-slug: ordersgroupsconfirm-post
  description: |-
    Returns estimated cost and commission information for a group of orders (OCO, BRK) without the orders actually being placed

    **Base Confirmation**  (All confirmations will have these fields)
    * Route
    * Duration
    * Account
    * SummaryMessage
    * OrderConfirmId

    **Equity Confirmation** (Base Confirmation fields + the following)
    * EstimatedPrice
    * EstimatedPriceDisplay
    * EstimatedCost
    * EstimatedCostDisplay
    * EstimatedCommission
    * EstimatedCommissionDisplay

    **Forex Confirmation** (Base Confirmation fields + the following)
    * BaseCurrency
    * CounterCurrency
    * InitialMarginDisplay

    **Futures Confirmation** (Base Confirmation fields + the following)
    * ProductCurrency
    * AccountCurrency
    * EstimatedCost
    * EstimatedPrice
    * EstimatedPriceDisplay
    * InitialMarginDisplay
    * EstimatedCommission
    * EstimatedCommissionDisplay
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/tradestation_logo_285x40.png
  humanURL: http://www.tradestation.com
  baseURL: https://api.tradestation.com//v2
  tags: Technology, Financial Services, Financial, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/groups/master/_listings/tradestation/ordersgroupsconfirm-post-openapi.md
x-common:
- type: x-website
  url: http://www.tradestation.com
- type: x-api-gallery
  url: http://tigertext.api.gallery.streamdata.io
- type: x-api-stack
  url: http://tradestation.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/tradestation-technologies
- type: x-developer
  url: https://developer.tradestation.com/
- type: x-documentation
  url: https://tradestation.github.io/api-docs/
- type: x-faq
  url: https://www.tradestation.com/faq/
- type: x-github
  url: https://github.com/tradestation
- type: x-openapi
  url: https://tradestation.github.io/api-docs/swagger.json
- type: x-pricing
  url: https://www.tradestation.com/pricing/
- type: x-twitter
  url: https://twitter.com/TradeStation
- type: x-website
  url: https://www.tradestation.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---