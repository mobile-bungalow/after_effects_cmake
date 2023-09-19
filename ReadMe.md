# After Effects Cmake Example

If you move this CmakeLists.txt into the Skeleton example in the AfterEffectsSDK you can run either of the following for 
cross platform builds.

### MacOS

```bash
take build
cmake .. -GXcode
xcodebuild
```

the resulting `Skeleton.plugin` signed bundle will be in the `/Debug` directory, you can pass the appropriate flags to produce a release package.

### Windows 

The following can be run from CMD, replacing "Visual Studio 17 2022" with your desired toolkit, and the path the the "MSBuild.exe" with the 
appropriate MSBuild.exe path. The resulting `Skeleton.aex` will be place in the `/Debug` output directory, you can pass the appropriate build flags to change the 
product type.

```bash
mkdir build
cd build
cmake .. -G "Visual Studio 17 2022" 
& 'c:\Program Files\Microsoft Visual Studio\2022\Community\MSBuild\Current\Bin\MSBuild.exe' .\Skeleton.sln
```

Alternatively, **just open this file in Visual Studio or vscode** with the CMake and CMake Tools plugins and you can use them to automatically configure and build the project. *This is probably the preferred method for most*, but driving from the command line is relevant for CI/CD purposes.
