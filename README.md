<h1 align="center">
 <img src="https://user-images.githubusercontent.com/45159366/120383684-09eb3280-c2da-11eb-9396-95b0f5696252.png">
  <br />
  Fuchsia Guide
</h1>

#### A guide covering Fuchsia including the applications, libraries and tools that will make you a better and more efficient Fuchsia developer.

**Note: You can easily convert this markdown file to a PDF in [VSCode](https://code.visualstudio.com/) using this handy extension [Markdown PDF](https://marketplace.visualstudio.com/items?itemName=yzane.markdown-pdf).**

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/120383768-21c2b680-c2da-11eb-8657-92f35f77959b.png">
  <br />
</p>

 # Table of Contents
 
 1. [Fuchsia Learning Resources](https://github.com/mikeroyal/Fuchsia-Guide#fuchsia-learning-resources)
 
 2. [Fuchsia Tools and Frameworks](https://github.com/mikeroyal/Fuchsia-Guide#fuchsia-tools-and-frameworks)
 
 3. [Flutter Development](https://github.com/mikeroyal/Fuchsia-Guide#flutter-development)
 
 4. [C/C++ Development](https://github.com/mikeroyal/Fuchsia-Guide#cc-development)
 
 5. [Dart Development](https://github.com/mikeroyal/Fuchsia-Guide#dart-development)
 
 6. [Rust Development](https://github.com/mikeroyal/Fuchsia-Guide#rust-development)
 
 7. [Go Development](https://github.com/mikeroyal/Fuchsia-Guide#go-development)
 
 8. [Python Development](https://github.com/mikeroyal/Fuchsia-Guide#python-development)

 9. [Wayland Development](https://github.com/mikeroyal/Fuchsia-Guide#wayland-development)
 
 
 <p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/120383693-0bb4f600-c2da-11eb-9876-2c5dae5f7b71.png">
  <br />
</p>

**Fuchsia OS on the Nest Hub . Source: [Google](https://store.google.com/product/nest_hub_2nd_gen?hl=en-US)**


 
# Fuchsia Learning Resources
[Back to the Top](https://github.com/mikeroyal/Fuchsia-Guide#table-of-contents)

[Fuchsia](https://fuchsia.dev/) is an open source effort to create a production-grade operating system that prioritizes security, updatability, and performance.

[Getting Started with Fuchsia](https://fuchsia.dev/fuchsia-src/get-started)

[Getting started with Zircon Kernel](https://fuchsia.dev/fuchsia-src/development/kernel/getting_started)

[Fuchsia APIs](https://fuchsia.dev/fuchsia-src/development#api)

[Supported Harware for Fuchsia](https://fuchsia.dev/fuchsia-src/development#hardware)

[Supported Programming Languages for Fuchsia](https://fuchsia.dev/fuchsia-src/development#languages)

[Fuchsia Reference](https://fuchsia.dev/reference)

[Contributing to Fuchsia](https://fuchsia.dev/fuchsia-src/CONTRIBUTING)

[Google Developers Training](https://developers.google.com/training/)

[Google Developers Certification](https://developers.google.com/certification/)

 
# Fuchsia Tools and Frameworks
[Back to the Top](https://github.com/mikeroyal/Fuchsia-Guide#table-of-contents)

[Fuchsia Filesystem Architecture](https://fuchsia.dev/fuchsia-src/concepts/filesystems/filesystems)

[Fuchsia emulator (FEMU)](https://fuchsia.dev/fuchsia-src/concepts/emulator) is the default emulator for Fuchsia. FEMU allows you to test Fuchsia components and applications without a physical Fuchsia device.

[Fuchsia Interface Definition Language (FIDL)](https://fuchsia.dev/fuchsia-src/concepts/fidl/overview) is the language used to describe interprocess communication (IPC) protocols used by programs running on Fuchsia.

[Fuchsia System Interface](https://fuchsia.dev/fuchsia-src/concepts/system/abi/system) is the binary interface that the Fuchsia operating system presents to software it runs. The foundation of the interface is the vDSO, which provides access to the system calls. Programs are not allowed to issue system calls directly (e.g., by trapping into the kernel). Instead, programs use the vDSO to interface with the kernel. The bulk of the system interface is provided through inter-process communication protocols, typically defined using FIDL. These protocols are spoken over various kernel primitives, including channels and sockets.

[Fuchsia Integrator Development Kit (IDK)](https://fuchsia.dev/docs/development/idk/gn) is a Developer Kit that contains a small set of libraries and tools required to start building and running programs that target Fuchsia.

[Zircon](https://fuchsia.dev/fuchsia-src/concepts/kernel) is the core platform that powers Fuchsia. Zircon is composed of a kernel (source in /zircon/kernel) as well as a small set of userspace services, drivers, and libraries (source in /zircon/system/) necessary for the system to boot, talk to hardware, load userspace processes and run them, etc. Fuchsia builds a much larger OS on top of this foundation.

[ffx](https://fuchsia.dev/fuchsia-src/development/tools/ffx/overview) is a tool that provides a unified platform for Fuchsia CLI tools for host target interactions. It introduces a service oriented interface to many common development and integration workflow operations that users may wish to perform against one or more Fuchsia target devices.

[Escher](https://fuchsia.dev/fuchsia-src/concepts/graphics/escher) is a physically based renderer. It is a C++/Vulkan library that is used primarily by the Scenic implementation; it is not exposed by the Fuchsia SDK.

[Magma](https://fuchsia.dev/fuchsia-src/concepts/graphics/magma) is the gpu driver architecture for Fuchsia. There are two driver components: a gpu-specific library loaded into each application’s address space; and the magma system driver that manages the hardware.

[Sysmem](https://fuchsia.dev/fuchsia-src/concepts/graphics/sysmem/sysmem) is a FIDL service that allocates shared memory for use by multiple applications and hardware blocks. This document gives an overview of its major features and what it provides to the system.

[GN](https://gn.googlesource.com/gn/) is a meta-build system that generates build files for [Ninja](https://ninja-build.org/). GN is currently used as the build system for Chromium, Fuchsia, and related projects. 

[GN C++ Frontend SDK](https://fuchsia.dev/fuchsia-src/development/idk/gn) is development kit that currently only supports Linux hosts and the [GN build system](https://gn.googlesource.com/gn/).


# Flutter Development

[Back to the Top](https://github.com/mikeroyal/Fuchsia-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/93719686-0abbaa00-fb39-11ea-978d-91e55844dd7a.png">
  <br />
</p>

## Flutter Learning Resources

[Flutter](https://flutter.dev/) is Google's UI toolkit for crafting beautiful, natively compiled applications for mobile(Andorid and iOS), web, and desktop(Windows, MacOS, Linux, and Google Fuchsia) from a single codebase. Flutter works with existing code, is used by developers and organizations around the world, and is free and open source.

[Flutter Gems](https://fluttergems.dev) is a curated package guide for Flutter which functionally categorizes some of the most useful and popular flutter packages available on pub.dev Flutter Gems A Flutter package landscape guide comprising 1500+ neatly categorized useful and popular packages.

[Dart](https://dart.dev/) is an open-source, scalable programming language, with robust libraries and runtimes, for building web, server, and mobile apps using the Flutter framework.

[Flutter documentation](https://flutter.dev/docs)

[Style Guide for Flutter](https://github.com/flutter/flutter/wiki/Style-guide-for-Flutter-repo)

[Creating your first Flutter app](https://flutter.dev/docs/get-started/codelab)

[Build and release an Android app using Flutter](https://flutter.dev/docs/deployment/android)

[Flutter Tools & techniques](https://flutter.dev/docs/development/tools)

[Dart and Flutter: The Complete Developer's Guide on Udemy](https://www.udemy.com/course/dart-and-flutter-the-complete-developers-guide/)

[Creating an Interactive Story with Flutter on Coursera](https://www.coursera.org/projects/story-creating-flutter)

[Flutter for Beginners course on Pluralsight](https://www.pluralsight.com/courses/flutter-getting-started)

[Flutter Online Training Courses on LinkedIn Learning](https://www.linkedin.com/learning/topics/flutter)

[The Complete Flutter App Development Bootcamp with Dart by App Brewery](https://www.appbrewery.co/p/flutter-development-bootcamp-with-dart)

[Adding Firebase to your Flutter app](https://firebase.google.com/docs/flutter/setup)

[Using Firebase and Firestore with Flutter](https://flutter.dev/docs/development/data-and-backend/firebase)

[Fuchsia Project](https://fuchsia.dev/)

[Getting Started with Fuchsia](https://fuchsia.dev/fuchsia-src/get-started)

[Fuchsia Reference](https://fuchsia.dev/reference)

[Contributing to Fuchsia](https://fuchsia.dev/fuchsia-src/CONTRIBUTING)

## Flutter Tools & Frameworks

[Firebase](https://firebase.google.com/) is a Backend-as-a-Service (BaaS) app development platform that provides hosted backend services such as a realtime database, cloud storage, authentication, crash reporting, machine learning, remote configuration, and hosting for your static files.

[FlutterFire](https://firebase.flutter.dev/) is a set of [Flutter plugins](https://flutter.io/platform-plugins/) that enable Flutter apps to use [Firebase](https://firebase.google.com/) services. You can follow an example that shows how to use these plugins in the [Firebase for Flutter](https://codelabs.developers.google.com/codelabs/flutter-firebase/index.html#0) codelab.

[FlutterBoost](https://github.com/alibaba/flutter_boost) is a Flutter plugin which enables hybrid integration of Flutter for your existing native apps with minimum efforts.

[Go-flutter](https://github.com/go-flutter-desktop/go-flutter) is a package that brings Flutter to the desktop. project implements the [Flutter's Embedding API](https://github.com/flutter/flutter/wiki/Custom-Flutter-Engine-Embedders) using a single code base that runs on Windows, macOS, and Linux. For rendering, [GLFW](https://github.com/go-gl/glfw) fits the job because it provides the right abstractions over the OpenGL's Buffer/Mouse/Keyboard for each platform.

[Appwrite](https://appwrite.io/) is a secure end-to-end backend server for Web, Mobile, and Flutter developers that is packaged as a set of Docker containers for easy deployment.

[Fluro](https://github.com/theyakka/fluro) is a Flutter routing library that adds flexible routing options like wildcards, named parameters and clear route definitions.
 
# C/C++ Development
[Back to the Top](https://github.com/mikeroyal/Fuchsia-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/115297894-961e0d80-a111-11eb-81c3-e2bd2ac9a7cd.png">
  <br />
 
</p>


## C/C++ Learning Resources

[C++](https://www.cplusplus.com/doc/tutorial/) is a cross-platform language that can be used to build high-performance applications developed by Bjarne Stroustrup, as an extension to the C language.

[C](https://www.iso.org/standard/74528.html) is a general-purpose, high-level language that was originally developed by Dennis M. Ritchie to develop the UNIX operating system at Bell Labs. It supports structured programming, lexical variable scope, and recursion, with a static type system. C also provides constructs that map efficiently to typical machine instructions, which makes it one was of the most widely used programming languages today.

[Embedded C](https://en.wikipedia.org/wiki/Embedded_C) is a set of language extensions for the C programming language by the [C Standards Committee](https://isocpp.org/std/the-committee) to address issues that exist between C extensions for different [embedded systems](https://en.wikipedia.org/wiki/Embedded_system). The extensions hep enhance microprocessor features such as fixed-point arithmetic, multiple distinct memory banks, and basic I/O operations. This makes Embedded C the most popular embedded software language in the world.

[C & C++ Developer Tools from JetBrains](https://www.jetbrains.com/cpp/)

[Open source C++ libraries on cppreference.com](https://en.cppreference.com/w/cpp/links/libs)

[C++ Graphics libraries](https://cpp.libhunt.com/libs/graphics)

[C++ Libraries in MATLAB](https://www.mathworks.com/help/matlab/call-cpp-library-functions.html)

[C++ Tools and Libraries Articles](https://www.cplusplus.com/articles/tools/)

[Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html)

[Introduction C++ Education course on Google Developers](https://developers.google.com/edu/c++/)

[C++ style guide for Fuchsia](https://fuchsia.dev/fuchsia-src/development/languages/c-cpp/cpp-style)

[C and C++ Coding Style Guide by OpenTitan](https://docs.opentitan.org/doc/rm/c_cpp_coding_style/)

[Chromium C++ Style Guide](https://chromium.googlesource.com/chromium/src/+/master/styleguide/c++/c++.md)

[C++ Core Guidelines](https://github.com/isocpp/CppCoreGuidelines/blob/master/CppCoreGuidelines.md)

[C++ Style Guide for ROS](http://wiki.ros.org/CppStyleGuide)

[Learn C++](https://www.learncpp.com/)

[Learn C : An Interactive C Tutorial](https://www.learn-c.org/)

[C++ Institute](https://cppinstitute.org/free-c-and-c-courses)

[C++ Online Training Courses on LinkedIn Learning](https://www.linkedin.com/learning/topics/c-plus-plus)

[C++ Tutorials on W3Schools](https://www.w3schools.com/cpp/default.asp)

[Learn C Programming Online Courses on edX](https://www.edx.org/learn/c-programming)

[Learn C++ with Online Courses on edX](https://www.edx.org/learn/c-plus-plus)

[Learn C++ on Codecademy](https://www.codecademy.com/learn/learn-c-plus-plus)

[Coding for Everyone: C and C++ course on Coursera](https://www.coursera.org/specializations/coding-for-everyone)

[C++ For C Programmers on Coursera](https://www.coursera.org/learn/c-plus-plus-a)

[Top C Courses on Coursera](https://www.coursera.org/courses?query=c%20programming)

[C++ Online Courses on Udemy](https://www.udemy.com/topic/c-plus-plus/)

[Top C Courses on Udemy](https://www.udemy.com/topic/c-programming/)

[Basics of Embedded C Programming for Beginners on Udemy](https://www.udemy.com/course/embedded-c-programming-for-embedded-systems/)

[C++ For Programmers Course on Udacity](https://www.udacity.com/course/c-for-programmers--ud210)

[C++ Fundamentals Course on Pluralsight](https://www.pluralsight.com/courses/learn-program-cplusplus)

[Introduction to C++ on MIT Free Online Course Materials](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-096-introduction-to-c-january-iap-2011/)

[Introduction to C++ for Programmers | Harvard ](https://online-learning.harvard.edu/course/introduction-c-programmers)

[Online C Courses | Harvard University](https://online-learning.harvard.edu/subject/c)


## C/C++ Tools

[Visual Studio](https://visualstudio.microsoft.com/) is an integrated development environment (IDE) from Microsoft; which is a feature-rich application that can be used for many aspects of software development. Visual Studio makes it easy to edit, debug, build, and publish your app. By using Microsoft software development platforms such as Windows API, Windows Forms, Windows Presentation Foundation, and Windows Store.

[Visual Studio Code](https://code.visualstudio.com/) is a code editor redefined and optimized for building and debugging modern web and cloud applications.

[Vcpkg](https://github.com/microsoft/vcpkg) is a C++ Library Manager for Windows, Linux, and MacOS.

[ReSharper C++](https://www.jetbrains.com/resharper-cpp/features/) is a Visual Studio Extension for C++ developers developed by JetBrains.

[AppCode](https://www.jetbrains.com/objc/) is constantly monitoring the quality of your code. It warns you of errors and smells and suggests quick-fixes to resolve them automatically. AppCode provides lots of code inspections for Objective-C, Swift, C/C++, and a number of code inspections for other supported languages. All code inspections are run on the fly.

[CLion](https://www.jetbrains.com/clion/features/) is a cross-platform IDE for C and C++ developers developed by JetBrains.

[Code::Blocks](https://www.codeblocks.org/) is a free C/C++ and Fortran IDE built to meet the most demanding needs of its users. It is designed to be very extensible and fully configurable. Built around a plugin framework, Code::Blocks can be extended with plugins.

[CppSharp](https://github.com/mono/CppSharp) is a tool and set of libraries which facilitates the usage of native C/C++ code with the .NET ecosystem. It consumes C/C++ header and library files and generates the necessary glue code to surface the native API as a managed API. Such an API can be used to consume an existing native library in your managed code or add managed scripting support to a native codebase.

[Conan](https://conan.io/) is an Open Source Package Manager for C++ development and dependency management into the 21st century and on par with the other development ecosystems. 

[High Performance Computing (HPC) SDK](https://developer.nvidia.com/hpc) is a comprehensive toolbox for GPU accelerating HPC modeling and simulation applications. It includes the C, C++, and Fortran compilers, libraries, and analysis tools necessary for developing HPC applications on the NVIDIA platform.

[Thrust](https://github.com/NVIDIA/thrust) is a C++ parallel programming library which resembles the C++ Standard Library. Thrust's high-level interface greatly enhances programmer productivity while enabling performance portability between GPUs and multicore CPUs. Interoperability with established technologies such as CUDA, TBB, and OpenMP integrates with existing software.

[Boost](https://www.boost.org/) is an educational opportunity focused on cutting-edge C++. Boost has been a participant in the annual Google Summer of Code since 2007, in which students develop their skills by working on Boost Library development.

[Automake](https://www.gnu.org/software/automake/) is a tool for automatically generating Makefile.in files compliant with the GNU Coding Standards. Automake requires the use of GNU Autoconf.

[Cmake](https://cmake.org/) is an open-source, cross-platform family of tools designed to build, test and package software. CMake is used to control the software compilation process using simple platform and compiler independent configuration files, and generate native makefiles and workspaces that can be used in the compiler environment of your choice.

[GDB](http://www.gnu.org/software/gdb/) is a debugger, that allows you to see what is going on `inside' another program while it executes or what another program was doing at the moment it crashed. 

[GCC](https://gcc.gnu.org/) is a compiler Collection that includes front ends for C, C++, Objective-C, Fortran, Ada, Go, and D, as well as libraries for these languages.

[GSL](https://www.gnu.org/software/gsl/) is a numerical library for C and C++ programmers. It is free software under the GNU General Public License. The library provides a wide range of mathematical routines such as random number generators, special functions and least-squares fitting. There are over 1000 functions in total with an extensive test suite.

[OpenGL Extension Wrangler Library (GLEW)](https://www.opengl.org/sdk/libs/GLEW/) is a cross-platform open-source C/C++ extension loading library. GLEW provides efficient run-time mechanisms for determining which OpenGL extensions are supported on the target platform.

[Libtool](https://www.gnu.org/software/libtool/) is a generic library support script that hides the complexity of using shared libraries behind a consistent, portable interface. To use Libtool, add the new generic library building commands to your Makefile, Makefile.in, or Makefile.am.

[Maven](https://maven.apache.org/) is a software project management and comprehension tool. Based on the concept of a project object model (POM), Maven can manage a project's build, reporting and documentation from a central piece of information.

[TAU (Tuning And Analysis Utilities)](http://www.cs.uoregon.edu/research/tau/home.php) is capable of gathering performance information through instrumentation of functions, methods, basic blocks, and statements as well as event-based sampling. All C++ language features are supported including templates and namespaces.

[Clang](https://clang.llvm.org/) is a production quality C, Objective-C, C++ and Objective-C++ compiler when targeting X86-32, X86-64, and ARM (other targets may have caveats, but are usually easy to fix). Clang is used in production to build performance-critical software like Google Chrome or Firefox.

[OpenCV](https://opencv.org/) is a highly optimized library with focus on real-time applications. Cross-Platform C++, Python and Java interfaces support Linux, MacOS, Windows, iOS, and Android.

[Libcu++](https://nvidia.github.io/libcudacxx) is the NVIDIA C++ Standard Library for your entire system. It provides a heterogeneous implementation of the C++ Standard Library that can be used in and between CPU and GPU code.

[ANTLR (ANother Tool for Language Recognition)](https://www.antlr.org/) is a powerful parser generator for reading, processing, executing, or translating structured text or binary files. It's widely used to build languages, tools, and frameworks. From a grammar, ANTLR generates a parser that can build parse trees and also generates a listener interface that makes it easy to respond to the recognition of phrases of interest.

[Oat++](https://oatpp.io/) is a light and powerful C++ web framework for highly scalable and resource-efficient web application. It's zero-dependency and easy-portable.

[JavaCPP](https://github.com/bytedeco/javacpp) is a program that provides efficient access to native C++ inside Java, not unlike the way some C/C++ compilers interact with assembly language. 

[Cython](https://cython.org/) is a language that makes writing C extensions for Python as easy as Python itself. Cython is based on Pyrex, but supports more cutting edge functionality and optimizations such as calling C functions and declaring C types on variables and class attributes.

[Spdlog](https://github.com/gabime/spdlog) is a very fast, header-only/compiled, C++ logging library. 

[Infer](https://fbinfer.com/) is a static analysis tool for Java, C++, Objective-C, and C. Infer is written in [OCaml](https://ocaml.org/).

# Dart Development
[Back to the Top](https://github.com/mikeroyal/Fuchsia-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/95024324-3067a980-0637-11eb-82bd-1c0b180c3fb3.png">
  <br />

</p>


## Dart Learning Resources

[Dart](https://dart.dev/) is an open-source, scalable programming language, with robust libraries and runtimes, for building web, server, and mobile apps using the [Flutter](https://flutter.dev/) framework.

[Dart API reference](https://api.dart.dev/stable/2.10.0/index.html)

[Dart core libraries](https://dart.dev/guides/libraries)

[Dart tutorials](https://dart.dev/tutorials)

[Getting Started with Dart SDK](https://dart.dev/get-dart)

[Creating a new Dart application with IntelliJ IDEA](https://www.jetbrains.com/help/idea/dart.html)

[Effective Dart Style Guide](https://dart.dev/guides/language/effective-dart/style#formatting)

[Learning Dart](https://reactdom.com/dart)

[Build Native Mobile Apps with Flutter on Udacity](https://www.udacity.com/course/build-native-mobile-apps-with-flutter--ud905)

[Dart for Beginners on Udemy](https://www.udemy.com/course/dartlang/)

[Dart Classes on Skilshare](https://www.skillshare.com/browse/dart-1?via=class-details-about-page)

[Fuchsia Project](https://fuchsia.dev/)

[Getting Started with Fuchsia](https://fuchsia.dev/fuchsia-src/get-started)

[Fuchsia Reference](https://fuchsia.dev/reference)

[Contributing to Fuchsia](https://fuchsia.dev/fuchsia-src/CONTRIBUTING)

## Dart Tools & Frameworks

[Android Studio](https://developer.android.com/studio/) is the official integrated development environment for Google's Android operating system, built on JetBrains' IntelliJ IDEA software and designed specifically for Android development. Availble on Windows, macOS, Linux, Chrome OS.

[IntelliJ IDEA](https://www.jetbrains.com/idea/) is an IDE for Java, but it also understands and provides intelligent coding assistance for a large variety of other languages such as Kotlin, SQL, JPQL, HTML, JavaScript, etc., even if the language expression is injected into a String literal in your Java code.

[Dart DevTools](https://dart.dev/tools/dart-devtools) is a suite of debugging and performance tools for Dart and Flutter. These tools are distributed in IDEs, the flutter tool, the webdev tool, and the [devtools package](https://pub.dev/packages/devtools).

[DartPad](https://www.dartpad.dev) is an online editor for Dart.

[Flutter SDK](https://flutter.dev/) is Google's UI toolkit for crafting beautiful, natively compiled applications for mobile, web, and desktop from a single codebase using Dart.

[Pub](https://dart.dev/tools/pub/cmd) is a  tool that has commands for managing packages and for deploying packages and command-line apps. 

[Analysis server](https://github.com/dart-lang/sdk/tree/master/pkg/analysis_server) is designed to provide on-going analysis of one or more code bases as those code bases are changing.

[Dart VM](https://dart.dev/tools/dart-vm) is a tool to run Dart command-line apps such as server-side scripts, programs, and servers.

[dart2js](https://dart.dev/tools/dart2js) is a tool to compile Dart code to deployable JavaScript. Another Dart-to-JavaScript compiler, [dartdevc](https://dart.dev/tools/dartdevc), is for development use only. The [webdev](https://dart.dev/tools/webdev#build) build command uses dart2js by default.

[dartdevc](https://dart.dev/tools/dartdevc) is the Dart development compiler that lets you run and debug your Dart web app in the Chrome browser.

[AngularDart](https://webdev.dartlang.org/angular) is a productive web application framework that powers some of Google's most critical applications. It's built on Dart and used extensively by Google AdWords, AdSense, Fiber, and many more projects.

[RxDart](https://pub.dev/packages/rxdart) is a package with Reactive Extensions for Dart that adds additional capabilities to Dart [Streams](https://api.dart.dev/stable/dart-async/Stream-class.html) and [StreamControllers](https://api.dart.dev/stable/dart-async/StreamController-class.html).


# Rust Development
[Back to the Top](https://github.com/mikeroyal/Fuchsia-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/119279024-f0613100-bbdd-11eb-9b52-30c276f8cc0f.png">
  <br />
 
</p>

 
## Rust Learning Resources

[Rust](https://www.rust-lang.org) is a multi-paradigm programming language focused on performance and safety. Rust has a comparable amount of runtime to C and C++, and has set up its standard library to be amenable towards OS development. Specifically, the standard library is split into two parts: core and std. Core is the lowest-level aspects only, and doesn't include things like allocation, threading, and other higher-level features.

[The Rust Language Reference](https://doc.rust-lang.org/nightly/reference/)

[The Rust Programming Language Book](https://doc.rust-lang.org/book/)

[Learning Rust](https://www.rust-lang.org/learn)

[Why AWS loves Rust](https://aws.amazon.com/blogs/opensource/why-aws-loves-rust-and-how-wed-like-to-help/)

[Rust Programming courses on Udemy](https://www.udemy.com/courses/search/?src=ukw&q=Rust)

[Safety in Systems Programming with Rust at Standford by Ryan Eberhardt](https://reberhardt.com/blog/2020/10/05/designing-a-new-class-at-stanford-safety-in-systems-programming.html)

[WebAssembly meets Kubernetes with Krustlet using Rust](https://cloudblogs.microsoft.com/opensource/2020/04/07/announcing-krustlet-kubernetes-rust-kubelet-webassembly-wasm/)

[Microsoft's Project Verona](https://github.com/microsoft/verona/blob/master/docs/explore.md)

## Rust Tools and Frameworks

[Cargo](https://github.com/rust-lang/cargo) is a package manager that downloads your Rust project’s dependencies and compiles your project.

[Crater](https://crater.rust-lang.org/) is a tool to run experiments across parts of the Rust ecosystem. Its primary purpose is to detect regressions in the Rust compiler, and it does this by building a large number of crates, running their test suites and comparing the results between two versions of the Rust compiler. It can operate locally (with Docker as the only dependency) or distributed on the cloud. It can operate locally (with Docker as the only dependency) or distributed on the cloud.

[VSCode-Rust](https://github.com/rust-lang/vscode-rust) is plugin that adds language support for Rust to Visual Studio Code. Rust support is powered by a separate language server - either by the official Rust Language Server (RLS) or rust-analyzer, depending on the user's preference. If you don't have it installed, the extension will install it for you (with permission). This extension is built and maintained by the Rust IDEs and editors team with the focus on providing a stable, high quality extension that makes the best use of the respective language server. 

[Apache Arrow](https://github.com/apache/arrow) is a development platform for in-memory analytics. It contains a set of technologies that enable big data systems to process and move data fast. Arrow's libraries are available for C, C++, C#, Go, Java, JavaScript, MATLAB, Python, R, Ruby, and Rust.

[Wasmer](https://wasmer.io/) enables super lightweight containers based on [WebAssembly](https://webassembly.org/) that can run anywhere such as the Desktop to the Cloud and IoT devices, and also embedded in [any programming language](https://github.com/wasmerio/wasmer#language-integrations).

[Firecracker](https://firecracker-microvm.github.io) is an open source virtualization technology that is purpose-built for creating and managing secure, multi-tenant container and function-based services that provide serverless operational models. Firecracker runs workloads in lightweight virtual machines, called microVMs, which combine the security and isolation properties provided by hardware virtualization technology with the speed and flexibility of containers. Firecracker has also been integrated in container runtimes, for example [Kata Containers](https://github.com/kata-containers/documentation/wiki/Initial-release-of-Kata-Containers-with-Firecracker-support) and [Weaveworks Ignite](https://github.com/weaveworks/ignite).

[Tokio](https://github.com/tokio-rs/tokio) is an event-driven, non-blocking I/O platform for writing asynchronous applications with the Rust programming language.

[TiKV](https://github.com/tikv/tikv) is an open-source distributed transactional key-value database that also provides classical key-vlue APIs, but also transactional APIs with ACID compliance.

[Sonic](https://crates.io/crates/sonic-server) is a fast, lightweight and schema-less search backend similar to Elasticsearch in some use-cases.

[Hyper](https://github.com/hyperium/hyper) is a fast and correct HTTP library for Rust.

[Rocket](https://github.com/SergioBenitez/Rocket) is an async web framework for Rust with a focus on usability, security, extensibility, and speed.

[Clippy](https://rust-lang.github.io/rust-clippy/) is a collection of lints to catch common mistakes and improve your Rust code.

[Servo](https://github.com/servo/servo) is a prototype web browser engine written in the Rust language.

[Vector](https://vector.dev/) is a high-performance, end-to-end (agent & aggregator) observability data platform that puts the user in control of their observability data.

[RustPython](https://github.com/RustPython/RustPython) is a Python Interpreter written in Rust.

[Miri](https://github.com/rust-lang/miri) is an interpreter for Rust's mid-level intermediate representation. It can run binaries and test suites of cargo projects and detect certain classes of undefined behavior. Miri will alsowill also tell you about memory leaks: when there is memory still allocated at the end of the execution, and that memory is not reachable from a global static, Miri will raise an error.

[Chalk](https://rust-lang.github.io/chalk/book/) is an implementation and definition of the Rust trait system using a PROLOG-like logic solver.

[stdarch](https://doc.rust-lang.org/stable/core/arch/) is Rust's standard library vendor-specific APIs and run-time feature detection.

[Simpleinfra](https://github.com/rust-lang/simpleinfra) is rep that contains the tools and automation written by the Rust infrastructure team to manage our services. Using some of the tools in this repo require privileges only infra team members have.

[Rustlings](https://github.com/rust-lang/rustlings) is a small set of exercises to get you used to reading and writing Rust code.

[Krustlet](https://krustlet.dev/) acts as a Kubernetes Kubelet(written in Rust) by listening on the event stream for new pods that the scheduler assigns to it based on specific Kubernetes [tolerations](https://kubernetes.io/docs/concepts/configuration/taint-and-toleration/). The project is currently experimental.

## Rust-based Operating Systems

[Redox](https://www.redox-os.org) is a Unix-like Operating System written in Rust, aiming to bring the innovations of Rust to a modern microkernel and full set of applications. Acitvely being developed by [Jeremy Soeller](https://gitlab.redox-os.org/jackpot51).

[Bottlerocket OS](https://github.com/bottlerocket-os/bottlerocket) is an open-source Linux-based operating system meant for hosting containers. Bottlerocket focuses on security and maintainability, providing a reliable, consistent, and safe platform for container-based workloads.

[Tock](https://www.tockos.org) is an embedded operating system designed for running multiple concurrent, mutually distrustful applications on Cortex-M and RISC-V based embedded platforms. Tock's design centers around protection, both from potentially malicious applications and from device drivers. Tock uses two mechanisms to protect different components of the operating system. First, the kernel and device drivers are written in Rust, a systems programming language that provides compile-time memory safety, type safety and strict aliasing. Tock uses Rust to protect the kernel (the scheduler and hardware abstraction layer) from platform specific device drivers as well as isolate device drivers from each other. Second, Tock uses memory protection units to isolate applications from each other and the kernel.

[Rust on Chrome OS](https://chromium.googlesource.com/chromiumos/docs/+/master/rust_on_cros.md) is a document that provides information on creating Rust projects for installation within Chrome OS and Chrome OS SDK. 

[Writing an OS in Rust ](https://os.phil-opp.com) is a blog series creates a small operating system in the Rust programming language by [Philipp Oppermann](https://github.com/phil-opp). 

# Go Development
[Back to the Top](https://github.com/mikeroyal/Fuchsia-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/93719679-068f8c80-fb39-11ea-8baa-9e779ee58a0a.png">
  <br />
  
</p>


## Go Learning Resources

[Go](https://golang.org/) is an open source programming language that makes it easy to build simple, reliable, and efficient software.

[Golang Contribution Guide](https://golang.org/doc/contribute.html)

[Google Developers Training](https://developers.google.com/training/)

[Google Developers Certification](https://developers.google.com/certification/)

[Uber's Go Style Guide](https://github.com/uber-go/guide/blob/master/style.md)

[GitLab's Go standards and style guidelines](https://docs.gitlab.com/ee/development/go_guide/)

[Effective Go](https://golang.org/doc/effective_go.html)

[Go: The Complete Developer's Guide (Golang) on Udemy](https://www.udemy.com/course/go-the-complete-developers-guide/)

[Getting Started with Go on Coursera](https://www.coursera.org/learn/golang-getting-started)

[Programming with Google Go on Coursera](https://www.coursera.org/specializations/google-golang)

[Learning Go Fundamentals on Pluralsight](https://www.pluralsight.com/courses/go-fundamentals)

[Learning Go on Codecademy](https://www.codecademy.com/learn/learn-go)

## Go Tools and Frameworks

[golang tools](https://pkg.go.dev/golang.org/x/tools) holds the source for various packages and tools that support the Go programming language.

[Go in Visual Studio Code](https://code.visualstudio.com/docs/languages/go) is an extension that gives you language features like IntelliSense, code navigation, symbol search, bracket matching, snippets, and many more that will help you in Golang development.

[Traefik](https://github.com/traefik/traefik) is a modern HTTP reverse proxy and load balancer that makes deploying microservices easy. Traefik integrates with your existing infrastructure components (Docker, Swarm mode, Kubernetes, Marathon, Consul, Etcd, Rancher, Amazon ECS, etc.) and configures itself automatically and dynamically. Pointing Traefik at your orchestrator should be the only configuration step you need.

[Gitea](https://github.com/go-gitea/gitea) is Git with a cup of tea, painless self-hosted git service. Using Go, this can be done with an independent binary distribution across all platforms which Go supports, including Linux, macOS, and Windows on x86, amd64, ARM and PowerPC architectures. 

[OpenFaaS](https://github.com/openfaas/faas) is Serverless Functions Made Simple. It makes it easy for developers to deploy event-driven functions and microservices to Kubernetes without repetitive, boiler-plate coding. Package your code or an existing binary in a Docker image to get a highly scalable endpoint with auto-scaling and metrics.

[micro](https://github.com/zyedidia/micro) is a terminal-based text editor that aims to be easy to use and intuitive, while also taking advantage of the capabilities of modern terminals. As its name indicates, micro aims to be somewhat of a successor to the nano editor by being easy to install and use. It strives to be enjoyable as a full-time editor for people who prefer to work in a terminal, or those who regularly edit files over SSH.

[Gravitational Teleport](https://github.com/gravitational/teleport) is a modern security gateway for remotely accessing into Clusters of Linux servers via SSH or SSH-over-HTTPS in a browser or Kubernetes clusters.

[NATS](https://nats.io/) is a simple, secure and performant communications system for digital systems, services and devices. NATS is part of the Cloud Native Computing Foundation (CNCF). NATS has over 30 client language implementations, and its server can run on-premise, in the cloud, at the edge, and even on a Raspberry Pi. NATS can secure and simplify design and operation of modern distributed systems.

[Act](https://github.com/nektos/act) is a GO program that allows you to run our GitHub Actions locally.

[Fiber](https://gofiber.io/) is an [Express](https://github.com/expressjs/express) inspired web framework built on top of [Fasthttp](https://github.com/valyala/fasthttp), the fastest HTTP engine for Go. Designed to ease things up for fast development with zero memory allocation and performance in mind. 

[Glide](https://github.com/Masterminds/glide) is a vendor Package Management for Golang.

[BadgerDB](https://github.com/dgraph-io/badger) is an embeddable, persistent and fast key-value (KV) database written in pure Go. It is the underlying database for [Dgraph](https://dgraph.io/), a fast, distributed graph database. It's meant to be a performant alternative to non-Go-based key-value stores like RocksDB.

[Go kit](https://github.com/go-kit/kit) is a programming toolkit for building microservices (or elegant monoliths) in Go. We solve common problems in distributed systems and application architecture so you can focus on delivering business value.

[Codis](https://github.com/CodisLabs/codis) is a proxy based high performance Redis cluster solution written in Go.

[zap](https://github.com/uber-go/zap) is a blazing fast, structured, leveled logging in Go. 

[HttpRouter](https://github.com/julienschmidt/httprouter) is a lightweight high performance HTTP request router (also called multiplexer or just mux for short) for Go.

[Gorilla WebSocket](https://github.com/gorilla/websocket) is a Go implementation of the WebSocket protocol.

[Delve](https://github.com/go-delve/delve) is a debugger for the Go programming language. 

[GORM](https://github.com/go-gorm/gorm) is a fantastic ORM library for Golang, aims to be developer friendly.

[Go Patterns](https://github.com/tmrts/go-patterns) is a curated collection of idiomatic design & application patterns for Go language.

# Python Development
[Back to the Top](https://github.com/mikeroyal/Fuchsia-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/93133273-ce490380-f68b-11ea-81d0-7f6a3debe6c0.png">
  <br />
  
</p>


## Python Learning Resources

[Python](https://www.python.org) is an interpreted, high-level programming language. Python is used heavily in the fields of Data Science and Machine Learning. 

[Python Developer’s Guide](https://devguide.python.org) is a comprehensive resource for contributing to Python – for both new and experienced contributors. It is maintained by the same community that maintains Python. 

[Azure Functions Python developer guide](https://docs.microsoft.com/en-us/azure/azure-functions/functions-reference-python) is an introduction to developing Azure Functions using Python. The content below assumes that you've already read the [Azure Functions developers guide](https://docs.microsoft.com/en-us/azure/azure-functions/functions-reference).

[CheckiO](https://checkio.org/) is a programming learning platform and a gamified website that teaches Python through solving code challenges and competing for the most elegant and creative solutions.

[Python Institute](https://pythoninstitute.org)

[PCEP – Certified Entry-Level Python Programmer certification](https://pythoninstitute.org/pcep-certification-entry-level/)

[PCAP – Certified Associate in Python Programming certification](https://pythoninstitute.org/pcap-certification-associate/)

[PCPP – Certified Professional in Python Programming 1 certification](https://pythoninstitute.org/pcpp-certification-professional/)

[PCPP – Certified Professional in Python Programming 2](https://pythoninstitute.org/pcpp-certification-professional/)

[MTA: Introduction to Programming Using Python Certification](https://docs.microsoft.com/en-us/learn/certifications/mta-introduction-to-programming-using-python)

[Getting Started with Python in Visual Studio Code](https://code.visualstudio.com/docs/python/python-tutorial)

[Google's Python Style Guide](https://google.github.io/styleguide/pyguide.html)

[Google's Python Education Class](https://developers.google.com/edu/python/)

[Real Python](https://realpython.com)

[The Python Open Source Computer Science Degree by Forrest Knight](https://github.com/ForrestKnight/open-source-cs-python)

[Intro to Python for Data Science](https://www.datacamp.com/courses/intro-to-python-for-data-science)

[Intro to Python by W3schools](https://www.w3schools.com/python/python_intro.asp)

[Codecademy's Python 3 course](https://www.codecademy.com/learn/learn-python-3)

[Learn Python with Online Courses and Classes from edX](https://www.edx.org/learn/python)

[Python Courses Online from Coursera](https://www.coursera.org/courses?query=python)

## Python Frameworks and Tools

[Python Package Index (PyPI)](https://pypi.org/) is a repository of software for the Python programming language. PyPI helps you find and install software developed and shared by the Python community. 

[PyCharm](https://www.jetbrains.com/pycharm/) is the best IDE I've ever used. With PyCharm, you can access the command line, connect to a database, create a virtual environment, and manage your version control system all in one place, saving time by avoiding constantly switching between windows.

[Python Tools for Visual Studio(PTVS)](https://microsoft.github.io/PTVS/) is a free, open source plugin that turns Visual Studio into a Python IDE. It supports editing, browsing, IntelliSense, mixed Python/C++ debugging, remote Linux/MacOS debugging, profiling, IPython, and web development with Django and other frameworks.

[Pylance](https://github.com/microsoft/pylance-release) is an extension that works alongside Python in Visual Studio Code to provide performant language support. Under the hood, Pylance is powered by Pyright, Microsoft's static type checking tool.

[Pyright](https://github.com/Microsoft/pyright) is a fast type checker meant for large Python source bases. It can run in a “watch” mode and performs fast incremental updates when files are modified.

[Django](https://www.djangoproject.com/) is a high-level Python Web framework that encourages rapid development and clean, pragmatic design.

[Flask](https://flask.palletsprojects.com/) is a micro web framework written in Python. It is classified as a microframework because it does not require particular tools or libraries. 
 
[Web2py](http://web2py.com/) is an open-source web application framework written in Python allowing allows web developers to program dynamic web content. One web2py instance can run multiple web sites using different databases.

[AWS Chalice](https://github.com/aws/chalice) is a framework for writing serverless apps in python. It allows you to quickly create and deploy applications that use AWS Lambda. 

[Tornado](https://www.tornadoweb.org/) is a Python web framework and asynchronous networking library. Tornado uses a non-blocking network I/O, which can scale to tens of thousands of open connections.

[HTTPie](https://github.com/httpie/httpie) is a command line HTTP client that makes CLI interaction with web services as easy as possible. HTTPie is designed for testing, debugging, and generally interacting with APIs & HTTP servers. 

[Scrapy](https://scrapy.org/) is a fast high-level web crawling and web scraping framework, used to crawl websites and extract structured data from their pages. It can be used for a wide range of purposes, from data mining to monitoring and automated testing.

[Sentry](https://sentry.io/) is a service that helps you monitor and fix crashes in realtime. The server is in Python, but it contains a full API for sending events from any language, in any application.

[Pipenv](https://github.com/pypa/pipenv) is a tool that aims to bring the best of all packaging worlds (bundler, composer, npm, cargo, yarn, etc.) to the Python world.

[Python Fire](https://github.com/google/python-fire) is a library for automatically generating command line interfaces (CLIs) from absolutely any Python object.

[Bottle](https://github.com/bottlepy/bottle) is a fast, simple and lightweight [WSGI](https://www.wsgi.org/) micro web-framework for Python. It is distributed as a single file module and has no dependencies other than the [Python Standard Library](https://docs.python.org/library/).

[CherryPy](https://cherrypy.org) is a minimalist Python object-oriented HTTP web framework.

[Sanic](https://github.com/huge-success/sanic) is a Python 3.6+ web server and web framework that's written to go fast. 

[Pyramid](https://trypyramid.com) is a small and fast open source Python web framework. It makes real-world web application development and deployment more fun and more productive.

[TurboGears](https://turbogears.org) is a hybrid web framework able to act both as a Full Stack framework or as a Microframework. 

[Falcon](https://falconframework.org/) is a reliable, high-performance Python web framework for building large-scale app backends and microservices with support for MongoDB, Pluggable Applications and autogenerated Admin.

[Neural Network Intelligence(NNI)](https://github.com/microsoft/nni) is an open source AutoML toolkit for automate machine learning lifecycle, including [Feature Engineering](https://github.com/microsoft/nni/blob/master/docs/en_US/FeatureEngineering/Overview.md), [Neural Architecture Search](https://github.com/microsoft/nni/blob/master/docs/en_US/NAS/Overview.md), [Model Compression](https://github.com/microsoft/nni/blob/master/docs/en_US/Compressor/Overview.md) and [Hyperparameter Tuning](https://github.com/microsoft/nni/blob/master/docs/en_US/Tuner/BuiltinTuner.md).

[Dash](https://plotly.com/dash) is a popular Python framework for building ML & data science web apps for Python, R, Julia, and Jupyter.

[Luigi](https://github.com/spotify/luigi) is a Python module that helps you build complex pipelines of batch jobs. It handles dependency resolution, workflow management, visualization etc. It also comes with Hadoop support built-in.

[Locust](https://github.com/locustio/locust) is an easy to use, scriptable and scalable performance testing tool. 

[spaCy](https://github.com/explosion/spaCy) is a library for advanced Natural Language Processing in Python and Cython. 

[NumPy](https://www.numpy.org/) is the fundamental package needed for scientific computing with Python.

[Pillow](https://python-pillow.org/) is a friendly PIL(Python Imaging Library) fork.

[IPython](https://ipython.org/) is a command shell for interactive computing in multiple programming languages, originally developed for the Python programming language, that offers enhanced introspection, rich media, additional shell syntax, tab completion, and rich history.

[GraphLab Create](https://turi.com/) is a Python library, backed by a C++ engine, for quickly building large-scale, high-performance machine learning models.

[Pandas](https://pandas.pydata.org/) is a fast, powerful, and easy to use open source data structrures, data analysis and manipulation tool, built on top of the Python programming language.

[PuLP](https://coin-or.github.io/pulp/) is an Linear Programming modeler written in python. PuLP can generate LP files and call on use highly optimized solvers, GLPK, COIN CLP/CBC, CPLEX, and GUROBI, to solve these linear problems.

[Matplotlib](https://matplotlib.org/) is a 2D plotting library for creating static, animated, and interactive visualizations in Python. Matplotlib produces publication-quality figures in a variety of hardcopy formats and interactive environments across platforms.

[Scikit-Learn](https://scikit-learn.org/stable/index.html) is a simple and efficient tool for data mining and data analysis. It is built on NumPy,SciPy, and mathplotlib.

#  Wayland Development
[Back to the Top](https://github.com/mikeroyal/Fuchsia-Guide#table-of-contents)

<p align="center">
 <img src="https://user-images.githubusercontent.com/45159366/104235197-79cf4e00-5409-11eb-97a6-a12f7bd8ad2a.png">
  <br />

</p>
 
## Wayland Learning Resources

[Wayland](https://wayland.freedesktop.org) is a protocol for a compositor to talk to its clients as well as a C library implementation of that protocol. The compositor can be a standalone display server running on Linux kernel modesetting and evdev input devices, an [X application](https://www.x.org/wiki/XServer/), or a wayland client itself.

[Wayland Architecture](https://wayland.freedesktop.org/architecture.html)

[Wayland Documentation](https://wayland.freedesktop.org/docs/html/)

[Sotfware Toolkits that have Wayland support right now](https://wayland.freedesktop.org/toolkits.html)

[Contribution instructions for Wayland](https://gitlab.freedesktop.org/wayland/wayland/blob/master/CONTRIBUTING.md)

[Contribution instructions for Weston](https://gitlab.freedesktop.org/wayland/weston/blob/master/CONTRIBUTING.md)

[Reporting Wayland bugs](https://gitlab.freedesktop.org/wayland/wayland/issues)

[Reporting Weston bugs](https://gitlab.freedesktop.org/wayland/weston/issues)

[WSLG: X11 and Wayland Applications in Windows Subsystem for Linux(WSL2)](https://linuxplumbersconf.org/event/9/contributions/611/attachments/702/1298/XDC2020_-_X11_and_Wayland_applications_in_WSL.pdf)

[Qt Wayland Compositor](https://doc.qt.io/qt-5/qtwaylandcompositor-index.html)

[Qt Wayland Compositor Examples](https://doc.qt.io/qt-5/qtwaylandcompositor-examples.html)

[Wayland on ArchWiki](https://wiki.archlinux.org/index.php/Wayland)

[Sway on ArchWiki](https://wiki.archlinux.org/index.php/Sway)

[Wayland on Ubuntu Wiki](https://wiki.ubuntu.com/Wayland)

[Wayland on Debian Wiki](https://wiki.debian.org/Wayland)

[The Wayland Display Server on Fedora Docs](https://docs.fedoraproject.org/en-US/fedora/rawhide/system-administrators-guide/Wayland/)

[Wayland features on Fedora Project Wiki](https://fedoraproject.org/wiki/Wayland_features)

[Wayland on GNOME Wiki](https://wiki.gnome.org/Initiatives/Wayland)

[KWin/Wayland on KDE Community Wiki](https://community.kde.org/index.php?title=KWin/Wayland)

[Wayland Desktop Landscape on Gentoo Wiki](https://wiki.gentoo.org/wiki/Wayland_Desktop_Landscape)

[Wayland in Void Linux Handbook](https://docs.voidlinux.org/config/graphical-session/wayland.html)

[Wayland on Enlightenment DE](https://www.enlightenment.org/about-wayland)

## Wayland Tools

[Weston](https://gitlab.freedesktop.org/wayland/weston) is a lightweight and functional Wayland compositor.

[XWayland](https://wayland.freedesktop.org/xserver.html) is an X Server running as a Wayland client(for backwards compatibility), allowing the [Xorg server](https://www.x.org/wiki/XServer/) can be modified to use wayland input devices for input and forward either the root window or individual top-level windows as wayland surfaces.

[KWayland](https://github.com/KDE/kwayland-server) is a Qt-style API to interact with the wayland-client and wayland-server API.

[Qt](https://www.qt.io/) is the faster, smarter way to create innovative devices, modern UIs & applications for multiple screens. It is one of the most popular toolkits for the Wayland and X11 windowing.

[GTK](https://www.gtk.org/) is a free and open source cross-platform widget toolkit for creating graphical user interfaces developed by [GNOME Project](https://www.gnome.org/). It is one of the most popular toolkits for the Wayland and X11 windowing.

[NVIDIA Wayland EGL External Platform library](https://github.com/NVIDIA/egl-wayland) is a work-in-progress implementation of a EGL External Platform library to add client-side Wayland support to EGL on top of EGLDevice and EGLStream families of extensions.

[NVIDIA EGL External Platform Interface](https://github.com/NVIDIA/eglexternalplatform) is a work-in-progress specification of the EGL External Platform interface for writing EGL platforms and their interactions with modern window systems on top of existing low-level EGL platform implementations. This keeps window system implementation specifics out of EGL drivers by using application-facing EGL functions.

[Sway](https://swaywm.org/) is an [i3](https://i3wm.org/)-compatible Wayland compositor. 

[wlroots](https://github.com/swaywm/wlroots) is a modular Wayland compositor library.

[WayfireWM](https://github.com/WayfireWM/wayfire) is a 3D Wayland compositor, inspired by [Compiz](https://launchpad.net/compiz) and based on [wlroots](https://github.com/swaywm/wlroots).

[SDDM](https://github.com/sddm/sddm) is a modern display manager for X11 and Wayland aiming to be fast, simple and beautiful. It uses modern technologies like QtQuick, which in turn gives the designer the ability to create smooth, animated user interfaces.

[x11docker](https://github.com/mviereck/x11docker) is an application that you allows to run graphical desktop applications (and entire desktops) in Docker Linux containers.

[Mako](https://github.com/emersion/mako) is alightweight notification daemon for Wayland. It also works on [Sway](https://swaywm.org/).

[Wayland-rs](https://github.com/Smithay/wayland-rs) is a Rust implementation of the wayland protocol (client and server).

[Wine-wayland](https://github.com/varmd/wine-wayland) is an application that allows you to running DX9/DX11 and Vulkan games using pure Wayland and Wine/DXVK.

## Contribute

- [x] If would you like to contribute to this guide simply make a [Pull Request](https://github.com/mikeroyal/Fuchsia-Guide/pulls).


## License

[Back to the Top](https://github.com/mikeroyal/Fuchsia-Guide/blob/main/README.md#table-of-contents)

Distributed under the [Creative Commons Attribution 4.0 International (CC BY 4.0) Public License](https://creativecommons.org/licenses/by/4.0/).
