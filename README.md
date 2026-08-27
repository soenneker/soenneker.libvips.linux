[![](https://img.shields.io/nuget/v/soenneker.libvips.linux.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libvips.linux/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libvips.linux/build-and-test.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libvips.linux/actions/workflows/build-and-test.yml)
[![](https://img.shields.io/nuget/dt/soenneker.libvips.linux.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libvips.linux/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libvips.linux/codeql.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libvips.linux/actions/workflows/codeql.yml)

# ![](https://user-images.githubusercontent.com/4441470/224455560-91ed3ee7-f510-4041-a8d2-3fc093025112.png) Soenneker.Libvips.Linux
### Provides the native libvips shared library for Linux x64.

## Installation

```
dotnet add package Soenneker.Libvips.Linux
```

The package places `libvips.so.42` under `runtimes/linux-x64/native`, so .NET selects and copies it for Linux x64 applications automatically.

The binary comes from [kleisauke/libvips-packaging](https://github.com/kleisauke/libvips-packaging). Third-party notices and exact component versions are included in the package.
