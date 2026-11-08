
# Quality Attribute Scenarios
## Project: Smart Unit Converter
Course: CMPS 570 – Software Architecture

### Main Quality Attribute: Testability

Testability is the ability to verify that the application works correctly through independent and automated testing.

### Scenario 1: Conversion Accuracy

- **Source:** User
- **Stimulus:** The user enters a value and selects two units to convert.
- **Environment:** Normal application operation.
- **Artifact:** Conversion Engine.
- **Response:** The system calculates and returns the correct converted value.
- **Response Measure:** 100% of predefined conversion test cases produce the expected results within an acceptable floating-point tolerance.

### Scenario 2: Independent Unit Testing

- **Source:** Developer
- **Stimulus:** The developer runs automated unit tests.
- **Environment:** Local development environment with the test framework installed.
- **Artifact:** Conversion modules.
- **Response:** Each conversion function runs independently without requiring the React interface.
- **Response Measure:** All conversion modules can be tested independently, and overall code coverage reaches at least 80%.

### Scenario 3: Easy Maintenance and Modification

- **Source:** Developer
- **Stimulus:** The developer adds a new unit or modifies an existing conversion formula.
- **Environment:** Application development and testing environment.
- **Artifact:** Conversion Engine and automated test modules.
- **Response:** The developer can update conversion logic without modifying unrelated UI components.
- **Response Measure:** Adding a new conversion unit requires changes only in the relevant conversion module and its tests, with all existing tests passing.
