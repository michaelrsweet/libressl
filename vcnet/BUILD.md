How To Build the Package
------------------------

This folder provides a build directory for LibreSSL on Windows using Visual
Studio, in order to produce NuGet packages others can use.

You need the following:

- Visual Studio 2019 or later
- NuGet command-line tools

Steps:

1. Build the Debug|x64 and Release|x64 configurations in Visual Studio.

2. Create the NuGet packages from a PowerShell window:

```
    nuget pack libressl_native.nuspec
    nuget pack libressl_native.redist.nuspec
```

3. Upload to NuGet.org.
