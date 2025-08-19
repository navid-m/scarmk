# net

*Source: `net.scar`*

## Imports

- `std/strings`

## Classes

### TcpServer

Represents some TCP server.

### TcpConnection

Represents some TCP connection.

### HttpRequest

Represents some HTTP request.

### HttpServer

Represents some HTTP server.

### HttpResponse

Represents some response from a HTTP request


## Functions

### socket_init

Initialize the socket library.

### socket_cleanup

Clean up the socket library.

### tcp_server_create

Create a TCP server.

### tcp_server_listen

Listen for incoming connections.

### tcp_server_accept

Accept an incoming connection.

### tcp_send

Send data over a TCP connection.

### tcp_receive

Receive data from a TCP connection.

### tcp_close

Close a TCP connection.

### tcp_server_close

Close a TCP server.

### http_parse_request

Parse an HTTP request.

### http_server_create

Create a HTTP server.

### http_server_start

Start the HTTP server.

### http_server_handle_request

Handle an HTTP request.

### http_json_response

Send a JSON response.

### http_html_response

Send an HTML response.

### url_encode

URL encode a string

### url_decode

URL decode a string

### http_get

Send a GET request to the specified URL and return the response

### http_post

Send a POST request to the specified URL and return the response

### http_put

HTTP PUT request

### http_delete

HTTP DELETE request

### download_file

Download a file from URL to local path

### ping_url

Check if a URL is reachable

