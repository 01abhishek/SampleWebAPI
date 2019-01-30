# SampleWebAPI
Sample Web API
This is a sample project which contains 2 web APIs. After cloning the files, if there are build errors then:
    Open the .csproj in a text editor and remove the below tag:
      <Target Name="EnsureNuGetPackageBuildImports" BeforeTargets="PrepareForBuild">
<PropertyGroup>
  <ErrorText>This project references NuGet package(s) that are missing on this computer. Use NuGet Package Restore to download them.  For more information, see http://go.microsoft.com/fwlink/?LinkID=322105. The missing file is {0}.</ErrorText>
</PropertyGroup>
<Error Condition="!Exists('..\..\..\Assemblies\NuGet\SpecFlow.Plus.Excel.1.4.2\build\SpecFlow.Plus.Excel.targets')" Text="$([System.String]::Format('$(ErrorText)', '..\..\..\Assemblies\NuGet\SpecFlow.Plus.Excel.1.4.2\build\SpecFlow.Plus.Excel.targets'))" />

Also run the command - update-Package –reinstall from the package manager console 
 
