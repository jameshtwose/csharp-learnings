# csharp-learnings
Looking into building C#/ .NET applications (and containerising with docker).

## Getting Started
### Prerequisites
Based on the following microsoft tutorial: https://learn.microsoft.com/en-us/dotnet/core/docker/build-container?tabs=linux&pivots=dotnet-7-0
- .NET 7+ SDK
  - If you have .NET installed, use the `dotnet --info` command to determine which SDK you're using.
- Docker Community Edition (CE)
  - If you have Docker installed, use the `docker --version` command to determine which version you're using.

### Running the application (locally - dotnet)
- `dotnet new console -o App -n DotNet.Docker`
- `cd App`
- `dotnet run`
- `ctrl + c` to stop the application (as it runs indefinitely)
- `dotnet publish -c Release` to publish the application

### Running the application (locally - docker)
- `cd App`
- `docker build -t dotnet-docker .`
- `docker run --rm dotnet-docker`