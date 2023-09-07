# Ranking Web App (developed with React and ASP.NET)

Required terminal code for vs code is provided below.

dotnet new react -n MyReactApp

cd MyReactApp

dotnet run

cd ClientApp

npm start

ClientApp/components/setuProxy.js -> change port to 7190

https://localhost:44453



# Jokes Web App (developed with ASP.NET core)

Required terminal code for vs code is provided below.

dotnet new mvc --auth Individual -n YourProjectName

dotnet run (run server)

https://localhost:7273 or http://localhost:5143

ctrl+c (end server)

// already installed -> dotnet tool install --global dotnet-aspnet-codegenerator

dotnet add package Microsoft.VisualStudio.Web.CodeGeneration.Design

dotnet add package Microsoft.EntityFrameworkCore

dotnet add package Microsoft.EntityFrameworkCore.SqlServer

dotnet clean

dotnet build

dotnet aspnet-codegenerator controller -name JokesController -m JokesWebApp.Models.Joke -dc JokesWebApp.Data.ApplicationDbContext --relativeFolderPath Controllers --useDefaultLayout –referenceScriptLibraries

dotnet ef migrations add MigrationName

dotnet ef database update



