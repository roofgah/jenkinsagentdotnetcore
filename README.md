# jenkinsagentdotnetcore
A jenkins build agent (slave) to build dotnet core 3.0 applications

This jenkins build is based on the `mcr.microsoft.com/dotnet/core/sdk:3.0.100-alpine3.9` so it will have all the .NET Core 3.0 SDK dependencies

Pull the docker image
```
docker pull roofgah/jenkinsagentdotnetcore
```
Run the container using
```
docker run -d roofgah/jenkinsagentdotnetcore -url <jenkins_url> <secret> <node-name>
```

Packages include:
* Openjdk 8
* Jenkins remoting 3.9
* .NET Core SDK 3.0.100
* GIT 
