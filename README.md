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

Check coverage check:

```commandline
go test -cover                                                                           ─╯
PASS
coverage: 75.0% of statements
ok      github.com/thegodeveloper/bookstore     0.473s
```

That means `75%` of the code is untested.

So, run the profile and generate the HTML report again. You should see:

```go
return Book{}, errors.New("no copies left")
```
