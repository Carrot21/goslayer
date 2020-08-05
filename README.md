# goslayer

## One statement intro

GoSLayer is a tool that helps you to create a golang project in seconds.

* layered base on a [standard architecture layout](https://github.com/golang-standards/project-layout) ([for chinese](https://github.com/danceyoung/paper-code/blob/master/package-oriented-design/packageorienteddesign.md))
* followed by [Package-Oriented-Design guideline](https://www.ardanlabs.com/blog/2017/02/package-oriented-design.html)
* creating a runnable Rest ful Web Service

## Usage

* `$ go get github.com/danceyoung/goslayer`
* cd any directory where you will creating your project: `$ goslayer`
* Enter your project name (here is `goapp`) and then choose a web framework(gin or http handler, default is gin)
* cd `goapp`: `go mod init goapp;go run ./cmd/myapp `
* Open another terminal, run `curl --location --request GET 'http://127.0.0.1:8080/goslayer/events'` , response data will output.

 Creation process and your project structure might look like this:

```
GoSLayer is a tool that helps you to create a golang project in seconds.

• layered base on a standard architecture layout
• followed by Package-Oriented-Design guideline
link: https://github.com/danceyoung/goslayer

Please enter your project name: goappPlease choose a web framework,
(1) use gin, (2) use handler buildin: 1

Creating your go project with GIN
The go project is created successfully.
goapp
├── cmd/
│   └── myapp/
│       └── router/
│           └── handler/
│           └── router.go
│       └── main.go
├── internal/
│   └── myapp/
│       └── event/
├── └── pkg/
│       └── middleware/
```

todo:

buildin http.handler or gin
router-biz

repository link

println project structure

usage

go check go install

cmd go mod tidy

cmd go run ./cmd/dd

unit test, integration test
