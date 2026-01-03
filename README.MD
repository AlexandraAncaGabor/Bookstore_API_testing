# Bookstore API Testing Suite

This project contains test cases and bug reports for a Bookstore API connected to a real database. The tests are organized into positive and negative scenarios and include manual test steps as well as Postman collections.  

> **Note:** This API testing project is related to the database project available [here](https://github.com/AlexandraAncaGabor/Database-queries/tree/main).

## Project Structure

### I. Test Cases
Manual test cases for positive and negative scenarios in Markdown format:

1. [Get_all_books.md](I.Test_cases/1.Get_all_books.md) – Get all books
2. [Post_new_user.md](I.Test_cases/2.Post_new_user.md) – Create a new user
3. [Post_new_review.md](I.Test_cases/3.Post_new_review.md) – Create a new review
4. [Delete_user.md](I.Test_cases/4.Delete_user.md) – Delete a user
5. [Get_book_invalid_id.md](I.Test_cases/5.Get_book_invalid_id.md) – Get a book with an invalid ID
6. [Post_user_invalid_id.md](I.Test_cases/6.Post_user_invalid_id.md) – Create a user with an invalid email
7. [Post_book_invalid_rating.md](I.Test_cases/7.Post_book_invalid_rating.md) – Create a book with an invalid rating
8. [Delete_book_invalid_id.md](I.Test_cases/8.Delete_book_invalid_id.md) – Delete a book with an invalid ID

### II. Postman Imported Tests
Postman collections for automated testing:

- **Negative_tests**  
  [Bookstore-api-testing.postman_collection.json](II.Postman_imported_tests/Negative_tests/Bookstore-api-testing.postman_collection.json) – contains negative test scenarios

- **Positive_tests**  
  [Bookstore-api-testing.postman_collection.json](II.Postman_imported_tests/Positive_tests/Bookstore-api-testing.postman_collection.json) – contains positive test scenarios

### III. Bugs
Documented bugs with reproduction steps and expected/actual results:

1. [Get_book_invalid_id.md](III.Bugs/1.Get_book_invalid_id.md) – Bug for GET book by invalid ID
2. [Delete_book_invalid_id.md](III.Bugs/2.Delete_book_invalid_id.md) – Bug for DELETE book by invalid ID

> **Note on Bugs:** The bugs documented above resulted from missing validation in the backend. Once proper validation is added these issues should be resolved.

## How to Run the Tests

1. Ensure the API server is running locally; 
2. For manual tests, follow the steps in each `.md` file.
3. For automated tests, import the Postman collections into Postman and run them.

## Notes

- Positive test cases ensure the API works as expected.
- Negative test cases are designed to identify potential bugs and error handling issues.
- Bugs are documented with expected vs. actual results, including screenshots if applicable.
- Postman collections can be found in [II.Postman_imported_tests](II.Postman_imported_tests)


✨ Guided by curiosity, committed to quality.
