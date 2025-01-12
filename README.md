# BulletSharp
BulletSharp is a .NET wrapper for the [Bullet](https://pybullet.org/) physics library.

This version uses Platform Invoke. There is also an equivalent version written in C++/CLI: https://github.com/AndresTraks/BulletSharp

libbulletc is a C interface to Bullet. It compiles into a .dll or .so file that exports Bullet functions.

BulletSharpPInvoke is a .NET library that proxies calls from .NET to libbulletc.

The benefit of P/Invoke over C++/CLI is that it runs on all platforms that support P/Invoke into shared user-mode libraries (Windows, Unix, Mac OS). See also [Supported platforms](https://github.com/AndresTraks/BulletSharp/wiki/Supported-platforms).

![.NET Core](https://github.com/AndresTraks/BulletSharpPInvoke/workflows/.NET%20Core/badge.svg)

# Changes in this fork
The source code is the same. The license is the same. I do not claim any ownership of the sources. The difference is that this does not use DLL maps, who still uses that in 2025 when we have modern cross-platform dotnet? I've also released a Nuget package because I could never get the original one to work under Linux. Furthermore, I've added native libraries for Mac x86_64 and ARM64.

# Installation
```
dotnet add package JAJ.Packages.BulletSharp --version 1.0.1
```