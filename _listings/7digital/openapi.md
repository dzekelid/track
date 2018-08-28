swagger: "2.0"
x-collection-name: 7digital
x-complete: 1
info:
  title: 7digital Purchasing API
  description: the-purchasing-api-allows-3rd-parties-to-deliver-digital-content-to-individual-users-
  version: "1.2"
host: api.7digital.com
basePath: 1.2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  track/chart:
    'get ':
      summary: track/chart
      description: This endpoint returns a chart of the most purchased tracks for
        given week. To retrieve the most recent charts as published on 7digital.com
        the toDate parameter should be omitted.
      operationId: trackchart
      x-api-path-slug: trackchart-get
      parameters:
      - ~
      - in: query
        name: country
        description: 2 letter ISO country code of the country whose tracks you would
          like to search
      - in: query
        name: imageSize
        description: The requested width of the image in pixels
      - in: query
        name: page
        description: Page number of the result set
      - in: query
        name: pageSize
        description: Number of items to be returned per page
      - in: query
        name: streamable
        description: If provided search results will contain only tracks that can/cannot
          be streamed
      - in: query
        name: toDate
        description: The last day the chart should include data for
      responses:
        200:
          description: OK
      tags:
      - Track
      - Chart
  user/purchase/{purchaseid}/track/{trackid}:
    'delete ':
      summary: user/purchase/{purchaseid}/track/{trackid}
      description: This method allows a user to remove a purchase of a track from
        the sales report when the purchase has been refunded.
      operationId: userpurchasepurchaseidtracktrackid
      x-api-path-slug: userpurchasepurchaseidtracktrackid-delete
      parameters:
      - ~
      - in: query
        name: purchaseid
        description: purchase id identifying the transaction at 7digitals end that
          the refunded item belongs to
      - in: query
        name: trackid
        description: nttttttttThe 7digital id of the track being refundednnttttttt
      responses:
        200:
          description: OK
      tags:
      - User
      - Purchase
      - Purchaseid
      - Track
      - Trackid