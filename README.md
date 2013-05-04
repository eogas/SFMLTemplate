What is SFMLTemplate?
====

SFMLTemplate is a basic Visual Studio 2012 project configured to build a "hello world" example for SFML.  The project
is configured by default to pull the required files from `C:\SFML-2.0` and `C:\SFML-2.0-x86` for 64 bit and 32 bit builds
respectively.  These values are stored, and can be easily changed, through the `$(SFMLDir)` variable defined in the
`SFMLTemplateX86` and `SFMLTemplateX64` property pages using Visual Studio's property manager.


Why is SFMLTemplate?
====

I figured this would be helpful for people like me who start a lot of projects that go nowhere.  People who frequently
start projects using the same stack may be annoyed at the overhead of configuring a working environment all the time,
so this project aims to serve as an easy way to get up and running without that overhead.


Other Info?
====

This project is configured to link the project dynamically, so it includes a post-build event that copies the .dlls from
the specified `$(SFMLDir)` into the output directory.
