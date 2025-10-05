# To Do List


---
## 1. Microsoft Solution Settings

### Editor Config



---

## Solution Structure
E


## 3. 

---

## 2. Naming Conventions

### Classes and Interfaces
- PascalCase for all class and interface names  
- Interfaces prefixed with `I` (e.g., `IUserService`)  
- Abstract classes suffixed with `Base` (e.g., `RepositoryBase`)  

### Methods and Properties
- PascalCase for public methods and properties  
- camelCase for private fields  
- Async methods suffixed with `Async`  

### Files and Folders
- Match file name to class name  
- Use plural folder names for logical groupings (e.g., `Models/`, `Services/`)  

---

## 3. Formatting and Style

- Use `var` when the type is obvious  
- Prefer expression-bodied members for simple properties and methods  
- Use `nameof()` instead of string literals for parameter names  
- Avoid regions unless necessary for collapsing large files  

---

## 4. Commenting and Documentation

### XML Comments
- Required for all public classes, methods, and properties  
- Use `<summary>`, `<param>`, and `<returns>` consistently
### Inline Comments
- Only for non-obvious logic  
- Avoid redundant or self-explanatory comments  

---

## 5. Testing Standards
These rule define the best practices and tools to use for writing unit and integration tests in Visual Studio solutions.
### Libraries and Tools
- **Test Framework**: Always use `MSTest` for unit and integration tests.
- **Mocks**: Use `Moq` to create mocks in unit tests.
### General Steps
1. **Unit Tests**:
   - Write tests for each valid and invalid scenario.
   - Use `Moq` to mock dependencies.
   - Verify exceptions and expected results.
   
2. **Integration Tests**:
   - Validate the entire business flow.

3. **Performance Tests**:
   - Add tests to validate the performance of critical features.
### Unit Tests
- Located in `[project].UnitTests/`.
- Test only the **Domain** and **Service** layers.
- Use `Moq` to mock dependencies.
- Do not interact with real databases or external services.
- Focus on business logic, use cases, and validation.
### Integration Tests
- Located in `[project].IntegrationTests/`.
- Test the **Infrastructure**, **Api**, and **Repository** layers, and the integration between layers.
- Validate the entire business flow, including data persistence and external calls.
### Best Practices
- Always write tests before implementation and follow test driven development (TDD) best practices.
- Document test cases in the corresponding files.
- Use explicit test names to describe their purpose.
### Additional Rule: Continuous Test Execution
- After every significant change or addition, run `dotnet test` or `dotnet watch` to verify the current state of the project.
- This ensures that all tests pass and helps identify issues early in the development process.
- Document the results of the test runs in the corresponding task or user story.

---




