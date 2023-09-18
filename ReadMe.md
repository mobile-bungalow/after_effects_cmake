# After Effects Cmake Example

If you move this CmakeLists.txt into the Skeleton example in the AfterEffectsSDK you can run either of the following for 
cross platform builds.

### For MacOS

```
take build
cmake .. -GXcode
xcodebuild
```

the resulting `Skeleton.plugin` signed bundle will be in the `/Debug` directory, you can pass the appropriate flags to produce a release package.



