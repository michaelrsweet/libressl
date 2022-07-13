How To Build the Package
------------------------

This folder provides a build directory for LibreSSL on Windows using Visual Studio, in
order to produce NuGet packages others can use.

You need the following:

- Visual Studio 2019 or later
- CMake 3.x or later
- NuGet command-line tools

Steps:

1. Update/create Visual Studio project files (as needed) with:

```
    cmake -D BUILD_SHARED_LIBS=yes ..
```

2. Build the Debug|x64 and Release|x64 configurations in Visual Studio.

3. Create the NuGet packages:

```
    nuget pack libressl_native.nuspec
    nuget pack libressl_native.redist.nuspec
```

4. Upload to NuGet.org.
