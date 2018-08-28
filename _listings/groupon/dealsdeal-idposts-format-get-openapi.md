---
swagger: "2.0"
x-collection-name: Groupon
x-complete: 0
info:
  title: Groupon Get Deals Deal Adds. Format
  description: Returns the lists of all the discussion posts for the specified deal.
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