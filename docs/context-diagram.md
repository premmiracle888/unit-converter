
# Context Diagram
## Project: Smart Unit Converter

The context diagram illustrates the interactions between the user, the Smart Unit Converter application, the web browser, and the developer's testing environment.

```mermaid
flowchart TB
    User["User"]
    Developer["Developer"]
    App["Smart Unit Converter<br/>React Web Application"]
    Browser["Web Browser"]
    Tests["Automated Test Suite<br/>Vitest"]

    User -->|"Enter values and select units"| Browser
    Browser -->|"Conversion request"| App
    App -->|"Converted result"| Browser
    Browser -->|"Display result"| User

    Developer -->|"Develop and maintain"| App
    Developer -->|"Run automated tests"| Tests
    Tests -->|"Test conversion logic"| App
    App -->|"Conversion functions"| Tests
    Tests -->|"Test results and coverage"| Developer
```
