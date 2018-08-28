---
swagger: "2.0"
x-collection-name: TradeStation
x-complete: 0
info:
  title: TradeStation Submit Group Order
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
  termsOfService: http://elasticbeanstalk-us-east-1-525856068889.s3.amazonaws.com/wp-content/uploads/2014/03/Guidelines_For_Acceptance.pdf
  contact:
    name: TradeStation API Team
    url: https://developer.tradestation.com/webapi
    email: webapi@tradestation.com
  version: 1.0.0
host: api.tradestation.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders/groups/confirm:
    post:
      summary: Confirm Group Order
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
      operationId: postOrderGroupsConfirm
      x-api-path-slug: ordersgroupsconfirm-post
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Confirm
      - Group
      - Order
  /orders/groups:
    post:
      summary: Submit Group Order
      description: "Submits a group order such as Bracket and OCO Orders.\n\n####
        Order Cancels Order (OCO)\nAn OCO order is a group of orders whereby if one
        of the orders is filled\nor partially-filled, then all of the other orders
        in the group are\ncancelled.\n\n#### Bracket OCO Orders\nA bracket order is
        a special instance of an OCO (Order Cancel Order).\nBracket orders are used
        to exit an existing position. They are designed\nto limit loss and lock in
        profit by ???bracketing??? an order with a\nsimultaneous stop and limit order.\n\nBracket
        orders are limited so that the orders are all for the same\nsymbol and are
        on the same side of the market (either all to sell or\nall to cover), and
        they are restricted to closing transactions.\n\nThe reason that they follow
        these rules is because the orders need to be\nable to auto decrement when
        a partial fill occurs with one of the orders.\nFor example, if the customer
        has a sell limit order for 1000 shares and\na sell stop order for 1000 shares,
        and the limit order is partially\nfilled for 500 shares, then the customer
        would want the stop to remain\nopen, but it should automatically decrement
        the order to 500 shares to\nmatch the remaining open position.\n\n### Errors\nWhen
        a submitted order fails, it can be seen in two different ways:\n-\tImmediately
        rejected during submit to the Orders API with a 400 HTTP status code.\n-\tAccepted
        by the API with a 200 HTTP status code, but you will see the order with a
        status of ???REJ??? (rejected) when you fetch the Order from the /v2/accounts/{id}/orders
        API\n\n#### NOTE\nWhen a group order is submitted, the order execution system
        treats each sibling order as an individual order. Thus, the system does not
        validate that each order has the same Quantity, and currently it is not able
        to update a bracket order as one transaction, instead you must update each
        order within a bracket.\n\nIn order to prevent errors, please validate the
        data on the client side."
      operationId: postOrderGroup
      x-api-path-slug: ordersgroups-post
      parameters:
      - in: query
        name: access_token
        description: A valid OAuth2 token used to authorize access to the resource
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Submit
      - Group
      - Order
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---