# discord-hacknaplan
A Discord bot that responds to mentions of Hacknplan tasks with embeds thereof

To load and run the pyproj, you need to create a file called CommandLineArguments.props and fill it with your secrets.
```XML
<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
    <PropertyGroup>
        <CommandLineArguments>--discord-token 0 --hacknplan-api-key 0 --hacknplan-project-id 0</CommandLineArguments>
    </PropertyGroup>
</Project>
```
