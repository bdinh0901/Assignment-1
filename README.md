# Getting Started
ZeroMQ microservice handles the ability to send a request to a server and then the server will then be able to serve data back to the client based on the request.  This microservice will supplement my partner's project by providing data in collaboration with my partner's UI.

Prerequisites
You will need the following items to use the service
- Python
- Zeromq installed in your python library
- UI needs to be synced to send requests to the server

# How the microservice send a request
- the UI will send the request based on the user's input to the server
- The server will then take the request and store it into a variable
- The UI will then send more request to further filter down the results that they are looking for
- The server will then receive those next requests and store them in a variable

SAMPLE CALL:
- User selects options in the first window and submits
- This will send a request to the server with the user's selection values
- The server will send back a request received message to allow the client to send more requests
- The user will then send more request based on how ever many selection screens the UI has
- As the UI sends in these requests the server is saving them in variables and then will return the expected results based on user selections



# How the microservice receives a request
- The server awaits for the UI to send a request
- Once a request is received the UI will then store the value in the request in a variable and send back a request received message (Server needs to send back response to allow the client tp send more requests)
- More requests are sent and their values are stored into variables as well
- Once all selections are made the Server will return a value based on what the user's inputs are that are stored in the variables

#UML Diagram
![CS361](https://user-images.githubusercontent.com/76972588/217996902-2f01d0f5-b416-4b69-96ac-4d2b98d0a986.jpeg)
