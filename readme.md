## petclinic

dotnet add package Npgsql.EntityFrameworkCore.PostgreSQL --version 7.0.4

dotnet tool update --global dotnet-ef --version 7.0.10

dotnet ef migrations add InitialMigration --context petclinic.Data.ApplicationDbContext -o "C:\Users\XXXXX\XXXXXXX\petclinic\Data\Migrations"

dotnet ef database update

dotnet ef migrations remove

## Modificar el login

dotnet aspnet-codegenerator identity -dc petclinic.Data.ApplicationDbContext --files "Account.Register;Account.Login"

dotnet add package Microsoft.VisualStudio.Web.CodeGeneration.Design --version 7.0.10