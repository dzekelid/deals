---
swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 0
info:
  title: Google Doubleclick API Delete Proposal Deal
  version: 1.0.0
  description: Delete the specified deals from the proposal
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /creatives/{accountId}/{buyerCreativeId}/addDeal/{dealId}:
    post:
      summary: Create Deal
      description: Add a deal id association for the creative.
      operationId: adexchangebuyer.creatives.addDeal
      x-api-path-slug: creativesaccountidbuyercreativeidadddealdealid-post
      parameters:
      - in: path
        name: accountId
        description: The id for the account that will serve this creative
      - in: path
        name: buyerCreativeId
        description: The buyer-specific id for this creative
      - in: path
        name: dealId
        description: The id of the deal id to associate with this creative
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
  /creatives/{accountId}/{buyerCreativeId}/listDeals:
    get:
      summary: List Deals
      description: Lists the external deal ids associated with the creative.
      operationId: adexchangebuyer.creatives.listDeals
      x-api-path-slug: creativesaccountidbuyercreativeidlistdeals-get
      parameters:
      - in: path
        name: accountId
        description: The id for the account that will serve this creative
      - in: path
        name: buyerCreativeId
        description: The buyer-specific id for this creative
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
  /creatives/{accountId}/{buyerCreativeId}/removeDeal/{dealId}:
    post:
      summary: Remove Deal
      description: Remove a deal id associated with the creative.
      operationId: adexchangebuyer.creatives.removeDeal
      x-api-path-slug: creativesaccountidbuyercreativeidremovedealdealid-post
      parameters:
      - in: path
        name: accountId
        description: The id for the account that will serve this creative
      - in: path
        name: buyerCreativeId
        description: The buyer-specific id for this creative
      - in: path
        name: dealId
        description: The id of the deal id to disassociate with this creative
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
  /proposals/{proposalId}/deals:
    get:
      summary: Get Proposal Deals
      description: List all the deals for a given proposal
      operationId: adexchangebuyer.marketplacedeals.list
      x-api-path-slug: proposalsproposaliddeals-get
      parameters:
      - in: query
        name: pqlQuery
        description: Query string to retrieve specific deals
      - in: path
        name: proposalId
        description: The proposalId to get deals for
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
  /proposals/{proposalId}/deals/delete:
    post:
      summary: Delete Proposal Deal
      description: Delete the specified deals from the proposal
      operationId: adexchangebuyer.marketplacedeals.delete
      x-api-path-slug: proposalsproposaliddealsdelete-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: proposalId
        description: The proposalId to delete deals from
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
  /proposals/{proposalId}/deals/insert:
    post:
      summary: Insert Proposal Deal
      description: Add new deals for the specified proposal
      operationId: adexchangebuyer.marketplacedeals.insert
      x-api-path-slug: proposalsproposaliddealsinsert-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: proposalId
        description: proposalId for which deals need to be added
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
  /proposals/{proposalId}/deals/update:
    post:
      summary: Update Proposal Deal
      description: Replaces all the deals in the proposal with the passed in deals
      operationId: adexchangebuyer.marketplacedeals.update
      x-api-path-slug: proposalsproposaliddealsupdate-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: proposalId
        description: The proposalId to edit deals on
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
  /accounts/{accountId}/preferreddeals:
    get:
      summary: Get Preferred Deals
      description: List the preferred deals for this Ad Exchange account.
      operationId: adexchangeseller.accounts.preferreddeals.list
      x-api-path-slug: accountsaccountidpreferreddeals-get
      parameters:
      - in: path
        name: accountId
        description: Account owning the deals
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
  /accounts/{accountId}/preferreddeals/{dealId}:
    get:
      summary: Get Preferred Deal
      description: Get information about the selected Ad Exchange Preferred Deal.
      operationId: adexchangeseller.accounts.preferreddeals.get
      x-api-path-slug: accountsaccountidpreferreddealsdealid-get
      parameters:
      - in: path
        name: accountId
        description: Account owning the deal
      - in: path
        name: dealId
        description: Preferred deal to get information about
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Deal
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