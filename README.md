# Tutorial and sample codes for ASP.NET 5 SPA with React

## Overview

This follows the following to create the default template codes.
- https://docs.microsoft.com/en-us/aspnet/core/client-side/spa/react?view=aspnetcore-5.0&tabs=netcore-cli

You can check the following for more detailed explanations.
- https://dev.to/packt/creating-spas-using-asp-net-core-and-react-59a0

The folder structure is the following
- my-new-app \ ClientApp folder: This is the React app. The build output in build folder will be served.
- my-new-app \ Controllers folder: This has a dummy Web API that the React app can send requests to.
   - To pass any data from the backend to the frontend, one shoud use the Web API. If the data is needed before the authentication, then one can create an API path without the need for authentication to pass the data that do not need to be protected.
- my-new-app \ Pages folder: This has some standard ASP.NET Razor pages.
- my-new-app \ Program.cs: This is the standard ASP.NET file.
- my-new-app \ Startup.cs: This specifies that this is serving the SPA static files from CilentApp \ build folder. This also sets up the Web API.
- my-new-app \ WeatherForcast.cs: This has the model used by the dummy Web API.

After the app is running, open https://localhost:5001 to see the web site.

## GitHub Actions included

- DOTNET build and test
- CodeQL

## Useful Visual Studio Code extensions

- https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.csharp
- https://marketplace.visualstudio.com/items?itemName=donjayamanne.githistory

## Useful Visual Studio Code references

- https://docs.microsoft.com/en-us/dotnet/core/tutorials/with-visual-studio-code#debug
- https://docs.microsoft.com/en-us/dotnet/core/tools/
- https://stackoverflow.com/questions/34275209/xml-auto-commenting-c-sharp-in-visual-studio-code
- https://stackoverflow.com/questions/47995468/vscode-c-sharp-go-to-definition-f12-not-working
- https://www.strathweb.com/2019/04/roslyn-analyzers-in-code-fixes-in-omnisharp-and-vs-code/

## Useful .NET CLI commands

- (Create the default template for backend and frontend) dotnet new react -o my-new-app
- (Powershell) SET ASPNETCORE_ENVIRONMENT=Development
- (in my-new-app folder) dotnet build 
- (in my-new-app folder) dotnet run
