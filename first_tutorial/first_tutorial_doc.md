<!--
 Copyright (c) 2022 Neşet Aydın
 
 This software is released under the MIT License.
 https://opensource.org/licenses/MIT
-->

# 1st Tutorial

## Create a folder and open in the terminal

```bash
mkdir first_tutorial && cd first_tutorial
```
## Import the folder in vscode
<kbd>Ctrl</kbd> + <kbd>K</kbd> + <kbd>O</kbd> and select your project path
## Create a dotnet project
- Firstly you paste this command, and check dotnetcore;
```bash
dotnet --info
```
Then you see a basic information about to .Net sdk on terminal:
```terminal
.NET SDK (reflecting any global.json):
 Version:   6.0.200
 Commit:    4c30de7899

Runtime Environment:
 OS Name:     ubuntu
 OS Version:  20.04
 OS Platform: Linux
 RID:         ubuntu.20.04-x64
 Base Path:   /usr/share/dotnet/sdk/6.0.200/

Host (useful for support):
  Version: 6.0.2
  Commit:  839cdfb0ec

.NET SDKs installed:
  6.0.200 [/usr/share/dotnet/sdk]

.NET runtimes installed:
  Microsoft.AspNetCore.App 6.0.2 [/usr/share/dotnet/shared/Microsoft.AspNetCore.App]
  Microsoft.NETCore.App 6.0.2 [/usr/share/dotnet/shared/Microsoft.NETCore.App]

To install additional .NET runtimes or SDKs:
  https://aka.ms/dotnet-download
```
Or you can check only verision
```bash
dotnet --version
```
Then the export on terminal as like be:
```terminal
6.0.200
```
You can learn the sub-commands with help command:
`bash dotnet --help` or `bash dotnet -h`

The sub-command outputs:
```terminal
.NET SDK (6.0.200)
Usage: dotnet [runtime-options] [path-to-application] [arguments]

Execute a .NET application.

runtime-options:
  --additionalprobingpath <path>   Path containing probing policy and assemblies to probe for.
  --additional-deps <path>         Path to additional deps.json file.
  --depsfile                       Path to <application>.deps.json file.
  --fx-version <version>           Version of the installed Shared Framework to use to run the application.
  --roll-forward <setting>         Roll forward to framework version  (LatestPatch, Minor, LatestMinor, Major, LatestMajor, Disable).
  --runtimeconfig                  Path to <application>.runtimeconfig.json file.

path-to-application:
  The path to an application .dll file to execute.

Usage: dotnet [sdk-options] [command] [command-options] [arguments]

Execute a .NET SDK command.

sdk-options:
  -d|--diagnostics  Enable diagnostic output.
  -h|--help         Show command line help.
  --info            Display .NET information.
  --list-runtimes   Display the installed runtimes.
  --list-sdks       Display the installed SDKs.
  --version         Display .NET SDK version in use.

SDK commands:
  add               Add a package or reference to a .NET project.
  build             Build a .NET project.
  build-server      Interact with servers started by a build.
  clean             Clean build outputs of a .NET project.
  format            Apply style preferences to a project or solution.
  help              Show command line help.
  list              List project references of a .NET project.
  msbuild           Run Microsoft Build Engine (MSBuild) commands.
  new               Create a new .NET project or file.
  nuget             Provides additional NuGet commands.
  pack              Create a NuGet package.
  publish           Publish a .NET project for deployment.
  remove            Remove a package or reference from a .NET project.
  restore           Restore dependencies specified in a .NET project.
  run               Build and run a .NET project output.
  sdk               Manage .NET SDK installation.
  sln               Modify Visual Studio solution files.
  store             Store the specified assemblies in the runtime package store.
  test              Run unit tests using the test runner specified in a .NET project.
  tool              Install or manage tools that extend the .NET experience.
  vstest            Run Microsoft Test Engine (VSTest) commands.
  workload          Manage optional workloads.

Additional commands from bundled tools:
  dev-certs         Create and manage development certificates.
  fsi               Start F# Interactive / execute F# scripts.
  sql-cache         SQL Server cache command-line tools.
  user-secrets      Manage development user secrets.
  watch             Start a file watcher that runs a command when files change.

Run 'dotnet [command] --help' for more information on a command.
```
Now, we create a .Net project in our path, firstly would go the path:
```bash
cd ~/csharp_tutorials/first_tutorial
```
And check our location in terminal:
```bash
pwd
```
The output must be as like this;
```terminal
/home/nesh/csharp_tutorials/first_tutorial
```
After the checking run this command;
```bash
dotnet new console
```
If dont a mistake, the outputs would be these;
```terminal
The template "Console App" was created successfully.

Processing post-creation actions...
Running 'dotnet restore' on /home/nesh/csharp_tutorials/first_tutorial/first_tutorial.csproj...
  Determining projects to restore...
  Restored /home/nesh/csharp_tutorials/first_tutorial/first_tutorial.csproj (in 94 ms).
Restore succeeded.
```
And dotnet has been create a obj folder, and a .csprojfile and .cs file, i 'll mention to files and folder but now, we try a print some words("Hello, aliens!") on terminal in the first tutorial.

- Now, open the **_Program.cs_** file;
```c#
// See https://aka.ms/new-console-template for more information
Console.WriteLine("Hello, World!");
```
You see a comment line and a Console.WriteLine method(this method works as similarly to std::cout or printf), i change the sentence and remove the comment line;
```c#
Console.WriteLine("Hello, Aliens!");
```
Lets try get to compile and run;
```bash
dotnet run
```
If dont any mistake, A **bin** (1) folder create in your path and you must see the output message;
```terminal
Hello, Aliens!
```

## Notes:
- (1) I ignore the bin folders in repo hense you couldn't find any bin folder.
