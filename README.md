# naming_guidelines UNDER CONSTRUCTION!


### Don't use "TX/RX" names for bidirectional transmissions (messages)
If you project have at list two nodes, and both of them can send and recive messages between each other, don't name this messages "RX/TX" or in any other way, that will flip it's name depending on which side to look from. What is output for sender is input for receiver.

#### Bad usage:
 * `TX/RX`
 * `send/receive`
 * `input/output`
 * `server/client` - almost good, but no meaning is it "to" or "from"
 * `to_client` - okay if you have only server-client connection, but bad if client_1->server->client_2 connection is possible
 * 

#### Good usage:
 * `to_server/to_requester` - 
 * `request/responce` - 

### The newest/oldest instead of "latest"
"Latest" record can be old and new. Instead this name it "new record", or "most recent" 
