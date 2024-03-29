﻿# New Project Template - HAVIT Blazor Stack

## Initial Setup
1. SetupSolution.ps1 - NewProjectTemplate => ProjectName
   1. Open SetupSolution.ps1 and set parameters.
   1. Run SetupSolution.ps1.
   1. Delete SetupSolution.ps1
1. Adjust the Model - remove unnecessary entities (Country, Localizations, ...)
1. Rebuild the solution
1. Run DataLayer CodeGenerator (Run-CodeGenerator.ps1)
1. Create an initial EF migration
   1. Drop the current migrations - delete Entity/Migrations folder
   1. Add new initial migration `Add-Migration Initial -StartupProject Entity.Tests`
1. Set Web.Server as the startup project.
1. Run the app...

## Further Steps
1. Update NuGet packages in solution.
1. Application Insights - set InstrumentationKey
	1. Web.Server / appSettings.json
    2. Web.Client / wwwroot / appSettings.json
2. Identity Server - set Keys for deployment (Web.Server / appSettings.json)

(Use PublishScripts folder for deployment settings.)

