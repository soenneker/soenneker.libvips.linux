[![](https://img.shields.io/nuget/v/soenneker.libvips.linux.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libvips.linux/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libvips.linux/build-and-test.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libvips.linux/actions/workflows/build-and-test.yml)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libvips.linux/publish-package.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libvips.linux/actions/workflows/publish-package.yml)
[![](https://img.shields.io/nuget/dt/soenneker.libvips.linux.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libvips.linux/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libvips.linux/codeql.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libvips.linux/actions/workflows/codeql.yml)

# Soenneker.Libvips.Linux

The libvips command-line distribution packaged for Linux x64 .NET applications.

## Install

```bash
dotnet add package Soenneker.Libvips.Linux
```

## Runtime files

The package copies `vips.sh`, `vips`, `vipsheader`, and their required runtime files beneath the application output directory:

```text
Resources/linux-x64/libvips/
```

Resolve that directory from `AppContext.BaseDirectory`; do not depend on the process working directory. This package contains Linux x64 assets only and does not select a distribution for other operating systems or architectures.

Most applications should reference `Soenneker.Libvips.Util`, which selects and invokes the matching platform tool. Reference this package directly when you need the native distribution without the managed wrapper.

The runtime comes from [kleisauke/libvips-packaging](https://github.com/kleisauke/libvips-packaging). Third-party notices and exact component versions are included in the package.
