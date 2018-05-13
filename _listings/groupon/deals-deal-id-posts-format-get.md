---
swagger: "2.0"
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
  /deals/{deal_id}/posts.{format}:
    get:
      summary: Get Deals Deal Adds. Format
      description: Returns the lists of all the discussion posts for the specified
        deal
      operationId: getDealsDealAdds.Format
      responses:
        200:
          description: OK
      tags:
      - deals
      - deal
      - posts
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