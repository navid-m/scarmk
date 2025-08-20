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

`socket_init() -> bool`

Initialize the socket library.

### socket_cleanup

`socket_cleanup() -> void`

Clean up the socket library.

### tcp_server_create

`tcp_server_create(i32 port) -> net`

Create a TCP server.

### tcp_server_listen

`tcp_server_listen(net::TcpServer server) -> bool`

Listen for incoming connections.

### tcp_server_accept

`tcp_server_accept(net::TcpServer server) -> net`

Accept an incoming connection.

### tcp_send

`tcp_send(net::TcpConnection conn, string data) -> i32`

Send data over a TCP connection.

### tcp_receive

`tcp_receive(net::TcpConnection conn, i32 max_size) -> lstring`

Receive data from a TCP connection.

### tcp_close

`tcp_close(net::TcpConnection conn) -> void`

Close a TCP connection.

### tcp_server_close

`tcp_server_close(net::TcpServer server) -> void`

Close a TCP server.

### http_parse_request

`http_parse_request(cstring raw_data) -> net`

Parse an HTTP request.

### http_server_create

`http_server_create(i32 port) -> net`

Create a HTTP server.

### http_server_start

`http_server_start(net::HttpServer server) -> bool`

Start the HTTP server.

### http_server_handle_request

`http_server_handle_request(net::TcpConnection conn, cstring response_body) -> void`

Handle an HTTP request.

### http_json_response

`http_json_response(net::TcpConnection conn, cstring json_body) -> void`

Send a JSON response.

### http_html_response

`http_html_response(net::TcpConnection conn, cstring html_body) -> void`

Send an HTML response.

### url_encode

`url_encode(cstring input) -> char*`

URL encode a string

### url_decode

`url_decode(char* str) -> char*`

URL decode a string

### http_get

`http_get(char* url) -> net`

Send a GET request to the specified URL and return the response

### http_post

`http_post(char* url, char* data) -> net`

Send a POST request to the specified URL and return the response

### http_put

`http_put(cstring url, cstring data) -> net`

HTTP PUT request

### http_delete

`http_delete(cstring url) -> net`

HTTP DELETE request

### download_file

`download_file(cstring url, cstring filepath) -> bool`

Download a file from URL to local path

### ping_url

`ping_url(cstring url) -> bool`

Check if a URL is reachable

