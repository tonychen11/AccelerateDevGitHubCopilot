# Library App

## Description
Library App is a console application designed to manage library operations such as searching for patrons, viewing patron details, and managing book loans. It utilizes a layered architecture with separate projects for core application logic, data access, and the console interface.

## Project Structure
- `AccelerateDevGitHubCopilot.sln`
- `README.md`
- `src/`
  - `Library.ApplicationCore/`
    - `Entities/`
    - `Enums/`
    - `Interfaces/`
    - `Services/`
    - `Library.ApplicationCore.csproj`
  - `Library.Console/`
    - `appSettings.json`
    - `CommonActions.cs`
    - `ConsoleApp.cs`
    - `ConsoleState.cs`
    - `Json/`
    - `Library.Console.csproj`
    - `Program.cs`
  - `Library.Infrastructure/`
    - `Data/`
    - `Library.Infrastructure.csproj`
- `tests/`
  - `UnitTests/`
    - `ApplicationCore/`
    - `UnitTests.csproj`

## Key Classes and Interfaces
- **Library.ApplicationCore**
  - `Entities/`
    - `Author`
    - `Book`
    - `BookItem`
    - `Loan`
    - `Patron`
  - `Enums/`
    - `CommonActions`
    - `ConsoleState`
  - `Interfaces/`
    - `ILoanRepository`
    - `ILoanService`
    - `IPatronRepository`
    - `IPatronService`
  - `Services/`
    - `LoanService`
    - `PatronService`
- **Library.Console**
  - `ConsoleApp`
  - `Program`
- **Library.Infrastructure**
  - `Data/`
    - `JsonData`
    - `JsonLoanRepository`
    - `JsonPatronRepository`

## Usage
1. Clone the repository.
2. Open the solution file `AccelerateDevGitHubCopilot.sln` in Visual Studio.
3. Build the solution to restore dependencies and compile the projects.
4. Run the `Library.Console` project to start the console application.
5. Follow the on-screen instructions to interact with the application.

## License
This project is licensed under the MIT License.