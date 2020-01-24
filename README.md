# NetEx
Extensions for the .Net Framework

[![Build status](https://ci.appveyor.com/api/projects/status/ajcp5ew8672akkme?svg=true)](https://ci.appveyor.com/project/Peckmore/netex)

This repository contains (hopefully!) useful extensions to the .Net Framework. This README serves as a quick overview of the functionality contained within the repository and how the project is structured.

## Overview

Each project is designed (where possible) to compile into it's own library based around a single set of functionality. For example, the *ProgressDialog* project will compile into a standalone library which provides progress dialog support.

All projects target the lowest framework version or standard possible in order to try and maximise compatibility with existing projects. Please note that projects will not all target *the same* framework version or standard, as some rely on functionality introduced in later versions.

## Nuget

All projects are available on NuGet. Each project is listed as a separate NuGet package so that you only need to add the functionality you require. The packages currently available are:

* [NetEx-CredentialDialog](https://www.nuget.org/packages/NetEx-CredentialDialog/)
* [NetEx-ProgressDialog](https://www.nuget.org/packages/NetEx-ProgressDialog/)

## Projects

The source for this repository is effectively split into two categories:

* **NetEx**: Projects which contain the extensions to the .Net Framework. This is the core of the repository.
* **NetExDemo**: Test projects which demonstrate the use of the **NetEx** projects.

### NetEx

**NetEx** currently contains the following projects:

* **CredentialDialog**: A managed implementation of the standard Windows credential dialog targeting .Net Framework 2.0.
* **CredentialDialogCore**: The same credential dialog project but targeting .Net Core 3.0.
* **ProgressDialog**: A managed implementation of the standard Windows progress dialog targeting .Net Framework 2.0.
* **ProgressDialogCore**: The same progress dialog project but targeting .Net Core 3.0.

### NetExDemo

**NetExDemo** currently contains the following projects:

* **NetExDemo**: A test project which demonstrates usage of the **NetEx** libraries targeting .Net Framework 2.0.
* **NetExDemoCore**: The same test project but targeting .Net Core 3.0.

##  License

The code is licensed under the [MIT license](https://github.com/Peckmore/NetEx/blob/master/LICENSE).