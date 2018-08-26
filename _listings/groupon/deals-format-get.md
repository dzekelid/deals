---
swagger: "2.0"
info:
  title: Groupon Get Deals. Format
  description: Returns an ordered list of deals that are currently launched for a
    specific division.
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
  /deals.{format}:
    get:
      summary: Get Deals. Format
      description: Returns an ordered list of deals that are currently launched for
        a specific division
      operationId: getDeals.Format
      responses:
        200:
          description: OK
      tags:
      - deals
      - format
definitions: []
x-collection-name: Groupon
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