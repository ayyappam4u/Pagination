# Pagination


When surfacing data from systems of record, one of the concerns designers and developers need to address is the potential of retrieving an enormous number of results in a single load session. This requires significant processing power on both the client and server sides and network traffic, and can degrade the overall data consumption and experience.

There are different approaches to address this concern, but one of the most widely used is the concept of pagination. 
Pagination is a term commonly used to describe the process of a sequential division of the contents (fetched data) into separate pages. 
This relieves the pressure on both sides of communication and its channel.

In MuleSoft, pagination is typically used when consuming APIs that return large amounts of data. 
When designing an integration in MuleSoft, need to ensure that your API client can efficiently handle paginated responses.
Here’s how you can implement pagination in MuleSoft, using the example of consuming a REST API with paginated responses.

    Databases (relational or NoSQL/Cache) are great examples of systems of records that support simple pagination by allowing developers to write commands to query paginated data.
    They require an OFFSET and a LIMIT, which determine where to start from and the maximum number of rows to be fetched.
