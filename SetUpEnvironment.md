### Install:  
https://nodejs.org/en/ latest stable preferably  
https://code.visualstudio.com/

### Create project:
- Create project folder <foldername>
- Enter folder dir
- Create solution for project
```sh 
dotnet new sln
```
- Create API project with -o parameter (Location to place the generated output)
```sh 
dotnet new webapi -o API
```
- Add project to solution
```sh 
dotnet sln add API
```
- Allow https support
```sh 
dotnet dev-certs https --trust
```

- Install EF globally
```sh 
https://www.nuget.org/packages/dotnet-ef/
```

- Create ef migrations file with -o parameter (Output path, recommended to use "Migrations name")
```sh
dotnet ef migrations add InitialCreate -o Data/Migrations
```

- Create db
```sh
dotnet ef database update
```

### Git
- Generate gitignore file with default values
```sh
dotnet new gitignore
```

### Visual Studio Code Extensions
- C#
- C# Extensions

### How to fix
- Intellisense in system language (polish)
1. Goto Intellisense folder, in my case
```sh 
C:\Users\MKL\.vscode\extensions\ms-dotnettools.csharp-1.23.4\.omnisharp\1.37.3\pl
```
2. Remove all dll files that start with "CodeAnalysis"