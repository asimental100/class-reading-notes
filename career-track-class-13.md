Mongo Aggregations
  1. The aggregation pipeline is a framework for data aggregation modeled on the concept of data processing pipelines. Documents enter a multi-stage pipeline that transforms the documents into aggregated results.
    1.a. First Stage: The $match stage filters the documents by the status field and passes to the next stage those documents that have status equal to "A".
    1.b. Second Stage: The $group stage groups the documents by the cust_id field to calculate the sum of the amount for each unique cust_id.
  2. In MongoDB, the aggregate command operates on a single collection, logically passing the entire collection into the aggregation pipeline. To optimize the operation, wherever possible, use the following strategies to avoid scanning the entire collection.

Aggregation by Example
  1. The aggregate function accepts an array of data transformations which are applied to the data in the order they're defined. This makes aggregation a lot like other data flow pipelines: the transformations that are defined first will be executed first and the result will be used by the next transformation in the sequence.
  2. he first stage of the pipeline is matching, and that allows us to filter out documents so that we're only manipulating the documents we care about. The matching expression looks and acts much like the MongoDB find function or a SQL WHERE clause.
  
