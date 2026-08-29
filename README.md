[![](https://img.shields.io/nuget/v/soenneker.libvips.linux.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libvips.linux/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libvips.linux/build-and-test.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libvips.linux/actions/workflows/build-and-test.yml)
[![](https://img.shields.io/nuget/dt/soenneker.libvips.linux.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libvips.linux/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libvips.linux/codeql.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libvips.linux/actions/workflows/codeql.yml)

# Soenneker.Libvips.Linux

Provides a bundled libvips command-line distribution for Linux x64.

## Install

```bash
dotnet add package Soenneker.Libvips.Linux
```

## What it provides

- Provides a bundled libvips command-line distribution for Linux x64.
- The package copies the distribution to `Resources/linux-x64/libvips`, including `vips.sh`, the `vips` and `vipsheader` executables, and their bundled runtime files.
- The runtime comes from [kleisauke/libvips-packaging](https://github.com/kleisauke/libvips-packaging). Third-party notices and exact component versions are included in the package.

## How to use it

Install the package, then consume the supplied build or runtime asset from your application. No service registration is required because this package exposes content rather than a callable API.
