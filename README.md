# Project Title

WCTC Example of using xUnit for unit testing

## Getting Started

Follow along in class and use this as a foundation for instruction

### Prerequisites

To create your own example, you can refer to the following Microsoft documentation.

```
[Unit testing C# in .NET Core using dotnet test and xUnit](https://docs.microsoft.com/en-us/dotnet/core/testing/unit-testing-with-dotnet-test)
```

### Installing

You can execute the following commands to create,

```
dotnet new sln -o unit-testing-using-dotnet-test
cd unit-testing-using-dotnet-test
dotnet new classlib -o PrimeService
ren .\PrimeService\Class1.cs PrimeService.cs
dotnet sln add ./PrimeService/PrimeService.csproj
dotnet new xunit -o PrimeService.Tests
dotnet add ./PrimeService.Tests/PrimeService.Tests.csproj reference ./PrimeService/PrimeService.csproj
dotnet sln add ./PrimeService.Tests/PrimeService.Tests.csproj
```

## Running the tests

To run the tests, change into the PrimeService.Tests directory and run the following command,

```
dotnet test
```

### Test Expectation

The tests are currently written to fail, and represent the idea of "Test Driven Development"

## Authors

* **Mark McArthey** - *Initial work* - [mcarthey](https://github.com/mcarthey/vscode-xunit-testing)

See also the top-level list of [repositories] (https://github.com/mcarthey?tab=repositories)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to Microsoft whose code was used

