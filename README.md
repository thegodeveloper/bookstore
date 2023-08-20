# Bookstore Project

This project is part of the `For the Love of Go` book, chapter `5. Story time`.

## Test Coverage

We can validate if all the code we have written was covered by our tests.

Generate a `coverage profile`:

```commandline
go test -coverprofile=coverage.out
```

Use this profile to generate an HTML page showing the covered code highlighted in `green`, uncovered in `red`, and ignored (things that aren't statements) in `grey`.

```commandline
go tool cover -html=coverage.out
```
