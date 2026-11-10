# Flutter Week 9 – REST API and JSON

Two Flutter exercises that request user records from the JSONPlaceholder demo API and display the returned data.

## Exercises

| File | Description |
|---|---|
| `9(a)` | Fetches users over HTTP, converts JSON objects into a Dart `User` model, and handles loading/error states |
| `9(b)` | Separates the user model and fetch function, including parsing and response validation |
| `output_9a.jpeg`, `output_9b.jpeg` | Screenshots of the exercise outputs |

## API used

The examples request `https://jsonplaceholder.typicode.com/users`. The response is a JSON array. Each exercise maps fields such as user ID, name and email (and phone in the second example) into Dart model objects.

## Concepts covered

- Making HTTP GET requests with the `http` package
- Decoding JSON with `jsonDecode`
- Mapping JSON maps into typed Dart objects
- Handling non-success response codes and malformed data
- Representing asynchronous loading and errors in the UI

## Run the examples

The repository stores extensionless source files and screenshots; it does not include a complete Flutter project.

```bash
flutter create rest_api_demo
cd rest_api_demo
flutter pub add http
```

Copy the selected exercise into `lib/main.dart` and run `flutter run`. Keep an internet connection available so the device can reach JSONPlaceholder.

## Learning objective

Practice connecting a Flutter interface to a REST endpoint, converting API data into typed models, and handling asynchronous network results.
