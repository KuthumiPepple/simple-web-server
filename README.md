# simple web server
This is a basic web server built using Go. It serves static files in the `static` directory and has two endpoints: `/hello` and `/form`.

## Installing dependencies
- This web server uses only one external dependency `net/http` which is a part of the standard Go library.

## Running the server
- Navigate to the root directory of the project
- Run `go run main.go`
- The server runs on port `8000`

## Endpoints
1. `/hello` (GET) - Returns "hello!" to the client if the URL path is `/hello` and the method is GET
2. `/form` (POST) - Returns the name and address submitted through a form

### `/hello`
- Expected response: `hello!`

### `/form`
- Method: POST
- Parameters:
    - `name` - Name of the person submitting the form
    - `address` - Address of the person submitting the form
- Expected response:
```
POST request successful
Name = {name}
Address = {address}
```
where `{name}` and `{address}` are the values submitted in the form.

**Note:** This is just a basic web server and should not be used for production purposes.