# Readme

This is a simple golang project which starts up a http server on port 4000. On opening the endpoint of the http server it gives an output `Hello docker` . This output can be changed to something else by setting up environment variables.

## Steps to Execute

* Clone the repository
* Golang 1.19 or higher version is required
* Execute the following commands
    ```
    go mod download
    go run main.go
    ```
* Open http://localhost:4000/ on browser. The default output will be `Hello docker`
* To modify the output run the following commands to export environment variable and run the execute the code.
    ```
    export DISPLAY_TEXT='<text>'
    go run main.go
    ```

## Build an executable binary

* To build an executable binary that can run on any linux environment:
    ```
    go build -o hello-docker
    ./hello-docker
    ```

## Environment Variable

**DISPLAY_TEXT** : To modify the output text to be printed