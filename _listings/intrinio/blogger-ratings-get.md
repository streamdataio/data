---
swagger: "2.0"
info:
  title: Intrinio API Blogger Ratings
  description: Returns blogger buy/sell/hold ratings for a specific security and date.
  version: 1.0.0
host: api.intrinio.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /blogger_ratings:
    get:
      summary: Blogger Ratings
      description: Returns blogger buy/sell/hold ratings for a specific security and
        date
      operationId: blogger-ratings
      parameters:
      - in: query
        name: blogger_id
        description: ' The ID of the blogger '
        type: string
      - in: query
        name: blog_id
        description: ' The ID of the blog '
        type: string
      - in: query
        name: identifier
        description: ' the identifier for the legal entity or a security associated
          with the company: '
        type: string
      - in: query
        name: page_number
        description: ' an integer greater than or equal to 1 for specifying the page
          number for the return values'
        type: string
      - in: query
        name: page_size
        description: ' an integer greater than 1 for specifying the number of results
          on each page'
        type: string
      - in: query
        name: rating
        description: ' The blogger rating (see section below) '
        type: string
      - in: query
        name: sector
        description: ' The name of the sector '
        type: string
      - in: query
        name: source
        description: ' The source of the data: tip'
        type: string
      responses:
        200:
          description: OK
      tags:
      - market data
      - blogger ratings
definitions: []
x-collection-name: Intrinio
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