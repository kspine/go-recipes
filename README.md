# Collection of Golang Recipes

[![Go Report Card](https://goreportcard.com/badge/github.com/cybersamx/go-recipes)](https://goreportcard.com/report/github.com/cybersamx/go-recipes)

I started this project as I was learning Go. Over time, it evolved into a handy reference for anyone to look up Go recipes and design patterns.

## Examples

Here is a collection of examples:

* [CLI](cli) - Setting commands, arguments, and flags when building a CLI program in Go.
  * [cobra](cli/cobra) - Implement a cli program using the cobra package.
  * [viper](cli/viper) - Passing configurations to a cli program using cli arguments, environment variables, and text file.
* [Collection](collection) - Go map, array, and slice.
  * [Array passing](collection/array-slice-passing) - An array is passed as a value to a function.
  * [Map](collection/map-basics) - Basic map operations.
  * [Slice](collection/slice-basics) - Basic slice operations.
  * [Sort](collection/sort) - Sort a slice of custom type elements.
* [Concurrency](concurrency) - Go concurrency.
  * [Channel](concurrency/channel)
    * [Basics](concurrency/channel/basics) - Basic channel examples.
    * [Buffered vs unbuffered channel](concurrency/channel/buffered-unbuffered) - Differences between buffered and unbuffered channels.
    * [Channel passing](concurrency/channel/channel-passing) - Message passing between 2 goroutines using a channel.
  * [WaitGroup](concurrency/waitgroup) - Using `sync.WaitGroup` to synchronize multiple concurrent goroutines.
* [Context](context) - The `context` package.
  * [Cancel](context/cancel) - Cancel contexts.
  * [Deadline](context/deadline) - Timeout using `context.WithDeadline` function.
* [Cookie](cookie) - Introduction to cookies in Go.
* [Dependency injection](di) - Different ways of implementing dependency injection using the `dig` and `wire` frameworks, and without a third-party framework.
* [Enum](enum) - Implement enum in Go.
* [Fake vs mock in unit testing](fake-mock) - The use of fake and mock in Go unit testing.
* [Generics](generics) - Go Generics.
  * [Custom type](generics/custom-type) - Using a custom type as a type parameter.
  * [Linked list](generics/linked-list) - Generic-based linked list.
  * [Type constraints](generics/type-constraints) -Type constraint basics.
  * [Type parameters](generics/type-parameters) - Type parameter basics.
* [GraphQL](graphql) - GraphQL in Go.
  * [GraphQL client](graphql/client) - A simple GraphQL client using the `machinebox/graphql` package.
  * [GraphQL server](graphql/server) - A simple GraphQL server using the `99designs/gqlgen` package.
* [gRPC](grpc) - GRPC examples.
  * [Hello world](grpc/hello-world) - A simple gRPC server-client setup.
  * [gRPC test](grpc/test) - Unit testing a gRPC server.
* [HTTP](http) - HTTP server.
  * [Client](http/client) - A simple HTTP client.
  * Server
    * [Form](http/server/form) - Handles a form submission (object binding and validation) using the gin framework.
    * [JWT](http/server/jwt) - Handles a simple web form submission and a simple authentication using JWT using the `dgrijalva/jwt-go` package.
    * [Static web server](http/server/static) - Implements a simple http server serving static content.
* [I/O](io) - Input/output operations.
  * [Basic read](io/basic-read) - Different ways to read.
  * [File reader](io/file-reader) - Different ways of reading from a file: incrementally and all-at-once.
  * [File writer](io/file-writer) - Writing to a file.
  * [Mutli-read](io/multi-read) - Reading from a source multiple times.
  * [Pipe](io/pipe) - Establish a pipeline for writing content on one end of the pipeline to reading on the end.
* [Long polling](long-poll) - A simple long-polling implementation.
* [MongoDB](mongo) - Working with MongoDB using the official Go driver.
  * [Basic](mongo/simple) - Basic operations with Mongo.
  * [Expiring data](mongo/expiring-data) - Remove expired data using MongoDB TTL indexing.
  * [Mongo operations](mongo/mongo-ops) - Run Mongo commands and other queries.
  * [Pre-defined schema](mongo/schema) - An example similar to the [basic mongo recipe](mongo/simple), but implemented using a pre-defined schema.
* [Pubsub](pubsub) - Pubsub examples.
  * [Kafka](pubsub/kafka) - A simple pubsub application using kafka.
* [Random](random) - Generating random data in Go.
* [Redis](redis) - recipes for working with Redis using the `mediocregopher/radix` and `go-redis/redis` drivers.
  * [Counter](redis/counter) - Global atomic counter that showcases basic operations in Redis.
  * [Sessions](redis/sessions) - Ephemeral sessions in Redis by setting up Redis to remove expired content using the [Go-Redis](https://redis.uptrace.dev/) and [Radix](https://github.com/mediocregopher/radix).
  * [Authentication](redis/auth) - Handling Redis authentication.
* [Reflection](reflect) - Go runtime reflection.
  * [Basics](reflect/basics) - Behaviors of reflection objects on different underlying values.
  * [Deep equal](reflect/equality) - Go (deep) equality operation using `reflect.DeepEqual` to compare 2 values.
  * [Merge map to struct](reflect/merge-fields) - Merge Matching Fields from Map to Struct.
  * [Merge map to struct recursively](reflect/merge-fields-recursive) - Same as the above merge map to struct with
    support for nested fields.
  * [Print fields](reflect/print-fields) - Print out the fields of a custom struct type.
  * [Set value](reflect/set-value) - Set a value on reflect.Value object.
* [Regular expression](regexp) - Regular expression basics.
* [Retry](retry) - Ways to implement retry in Go.
  * [Standard](retry/standard) - Simple retry implemented using Go, no third-party package.
  * [Retry package](retry/retry) - Retry using the `flowchartsman/retry` package.
* [Scheduler](scheduler) - Ways to schedule code to run periodically in the background.
* [Serialization](serialization) - Go serialization.
  * [CSV](serialization/csv) - Write and read csv files.
  * [JSON](serialization/json) - Basic json serialization using `json.MarshalJSON()` and `json.UnmarshalJSON()` functions.
* [System](system) - System.
  * [Interrupt via channel](system/interrupt) - Get notify of a system interrupt via channels.
* [SQL](sql) - Connecting to a relational database.
  * [Ephemeral SQL data model](sql/ephemeral-sql-data) - SQL garbage collector that removes expired records in sql database.
  * [SQL](sql/sql) - Connect to Postgres using the `database/sql` package.
  * [SQLite](sql/sqlite) - Connect to a SQLite database.
* [String](string) - Strings and characters in Go.
  * [Count iterate](string/count-iterate) - Count and iterate over a string by rune and byte.
  * [Unicode](string/unicode) - Unicode basics.
* [Template](template) - Go template.
  * [HTML template](template/html) - Server-side web content rendering using the `html/template` package.
  * [Layouts](template/layouts) - Create reusable templates (aka layouts).
* [Testing](testing) - Go testing.
  * [T.Helper](testing/helper) - What is T.Helper() and what it does.
* [Time](time) - Datetime in Go.
  * [Parse](time/parse) - Parses a date string to a Go struct value.
  * [Print](time/print) - Prints a date value to different formats.
* [Type check](typecheck) - Type checking at runtime.
* [Validation](validation) - Sample code for the `go-playground/validator` package.
* [WebAssembly](wasm) - A simple web assembly that prints "hello world" in the browser console.
* [Webhook](webhook) - The client will push a random event message to a webhook endpoint on the sever every 5 seconds.

