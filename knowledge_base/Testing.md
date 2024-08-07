# Testing

Date: Sunday, January 14, 2024

Time: 9:22 PM

## Topics

- Use assert statements
- Metrics
  - 90<sup>th</sup> percentile
- Test cases
  - Expected user behaviour – happy path testing
  - Corner Cases
  - Is proper error handling done?

## Types of Testing

- White box Testing
- Black box Testing
- Unit Testing
  - Code Coverage
  - Operation mutation
  - Try to make the test fail
  - [Property based testing](https://youtu.be/IYzDFHx6QPY?si=sFn5a3PBlfd9knRD)
    - Random value property based testing
    - Different path, same destination (mapping an array and sorting == sorting an array and mapping)
    - Invert the operation, check for original input (reverse a list two times, you get original one)
  - [Effective Unit Testing](https://youtu.be/fr1E9aVnBxw?si=MAh5aqCtBYBr5SXb)
    - Run quick tests first
    - [Follow TDD](https://youtu.be/vXnTMjMe5Eg?si=GVI9QhWBRAk2RxHH)
      - Write test first
      - Run the test, it should fail
      - Write code to pass the test
    - Avoid test interdependency, run them parallely
- Integration Testing
- End to end Testing
- Performance Testing

## Case Studies

Explore how popular open-source libraries write tests:

- Langchain
  - Folders for unit and integration tests, where app structure is maintained
  - [Langchain test docs](https://python.langchain.com/v0.1/docs/contributing/testing/)
    - prefers unit tests over integration tests
    - unit tests run on every PR
    - integration tests runs once a day
      - http interaction will be cached using pytest-vcr - [ref](https://python.langchain.com/v0.1/docs/contributing/testing/#recording-http-interactions-with-pytest-vcr)
    - llm is mocked while testing agents

Explore how tests written in Astro:

- Frontend
- Backend
- AI

# Explore
- Qmetry