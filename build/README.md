# Build and Packaging Instructions

1. Open a Terminal with Administrative Privileges
1. Change to the `{repo}\build` directory
1. From powershill, enter the following to build and package to zip

    ~~~bash
    & "C:\Program Files (x86)\Microsoft Visual Studio\2019\Community\MSBuild\Current\Bin\msbuild.exe" .\build.proj /t:PreparePackageModern /p:ReleaseVersion=2021.04.02
    & "C:\Program Files (x86)\Microsoft Visual Studio\2019\Community\MSBuild\Current\Bin\msbuild.exe" .\build.proj /t:Package /p:ReleaseVersion=2021.04.02
    ~~~

1. The zip archive is found in the `{repo}\build` directory.