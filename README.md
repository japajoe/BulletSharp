# BulletSharp
BulletSharp is a .NET wrapper for the [Bullet](https://pybullet.org/) physics library.

This version uses Platform Invoke. There is also an equivalent version written in C++/CLI: https://github.com/AndresTraks/BulletSharp

libbulletc is a C interface to Bullet. It compiles into a .dll or .so file that exports Bullet functions.

BulletSharpPInvoke is a .NET library that proxies calls from .NET to libbulletc.

The benefit of P/Invoke over C++/CLI is that it runs on all platforms that support P/Invoke into shared user-mode libraries (Windows, Unix, Mac OS). See also [Supported platforms](https://github.com/AndresTraks/BulletSharp/wiki/Supported-platforms).

![.NET Core](https://github.com/AndresTraks/BulletSharpPInvoke/workflows/.NET%20Core/badge.svg)

# Changes in this fork
The source code is the same. The license is the same. I do not claim any ownership of the sources. The difference is that this does not use DLL maps and has more target platforms.

# Installation
```
dotnet add package JAJ.Packages.BulletSharp --version 1.0.2
```

# Changes in 1.0.2
- Provide correct binary for Mac x86_64
- Add Linux ARM and ARM64.