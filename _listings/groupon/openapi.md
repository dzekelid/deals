---
swagger: "2.0"
x-collection-name: Groupon
x-complete: 1
info:
  title: Groupon API2
  description: put-all-those-great-ideas-for-groupon-improvements-extensions-and-multipleplatform-interfaces-to-work-
  version: v2
host: api.groupon.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /deals/{id}.{format}:
    parameters:
      summary: Parameters Deals . Format
      description: Parameters deals . format.
      operationId: parametersDeals.Format
      x-api-path-slug: dealsid-format-parameters
      responses:
        200:
          description: OK
      tags:
      - Deals
      - Format
    get:
      summary: Get Deals . Format
      description: Returns the detailed information about a specified deal.
      operationId: getDeals.Format
      x-api-path-slug: dealsid-format-get
      responses:
        200:
          description: OK
      tags:
      - Deals
      - Format
  /deals.{format}:
    parameters:
      summary: Parameters Deals. Format
      description: Parameters deals. format.
      operationId: parametersDeals.Format
      x-api-path-slug: deals-format-parameters
      responses:
        200:
          description: OK
      tags:
      - Deals
      - Format
    get:
      summary: Get Deals. Format
      description: Returns an ordered list of deals that are currently launched for
        a specific division.
      operationId: getDeals.Format
      x-api-path-slug: deals-format-get
      responses:
        200:
          description: OK
      tags:
      - Deals
      - Format
  /deals/{deal_id}/posts.{format}:
    parameters:
      summary: Parameters Deals Deal Adds. Format
      description: Parameters deals deal adds. format.
      operationId: parametersDealsDealAdds.Format
      x-api-path-slug: dealsdeal-idposts-format-parameters
      responses:
        200:
          description: OK
      tags:
      - Deals
      - Deal
      - Posts
      - Format
    get:
      summary: Get Deals Deal Adds. Format
      description: Returns the lists of all the discussion posts for the specified
        deal.
      operationId: getDealsDealAdds.Format
      x-api-path-slug: dealsdeal-idposts-format-get
      responses:
        200:
          description: OK
      tags:
      - Deals
      - Deal
      - Posts
      - Format
---