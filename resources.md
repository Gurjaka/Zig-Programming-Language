# Zig Learning Resources 🔥

A curated collection of resources for learning Zig, organized by learning stage and topic.

## 🚀 Getting Started (Absolute Beginners)

### Essential First Steps
- **[Zig Learn](https://ziglearn.org/)** ⭐ **Start here!**
  - Comprehensive online guide covering all basics
  - Well-structured chapters with practical examples
  - Updated regularly, covers modern Zig idioms

- **[Ziglings](https://codeberg.org/ziglings/exercises)** ⭐ **Must-do exercises**
  - Interactive coding exercises that teach Zig step-by-step
  - Perfect for hands-on learners
  - Builds muscle memory for Zig syntax and concepts

- **[Official Zig Documentation](https://ziglang.org/documentation/master/)**
  - Authoritative language reference
  - Dense but comprehensive
  - Great for looking up specific features

## 📚 Learning Resources by Topic

### Language Fundamentals
- **[Zig by Example](https://zig-by-example.github.io/)**
  - Code-first learning approach
  - Shows idiomatic patterns
  - Quick reference for common tasks

- **[Zig Guide (GitHub)](https://github.com/Sobeston/zig-learn)**
  - Source code for ziglearn.org
  - Additional examples and community contributions

### Memory Management & Allocators
- **[Allocators in Zig](https://ziglearn.org/chapter-2/#allocators)**
  - Essential for systems programming
  - Different allocator types and when to use them

- **[Memory Management Patterns](https://github.com/ziglang/zig/wiki/Memory-Management)**
  - Community wiki on memory best practices
  - Real-world allocation patterns

### Comptime (Compile-time Code Execution)
- **[Comptime in Zig Learn](https://ziglearn.org/chapter-2/#comptime)**
  - Introduction to Zig's compile-time magic
  - Generic programming and metaprogramming

- **[Advanced Comptime Patterns](https://kristoff.it/blog/what-is-zig-comptime/)**
  - Deep dive into comptime concepts
  - Written by Zig core team member

### C Interoperability
- **[Interfacing with C](https://ziglearn.org/chapter-4/)**
  - Essential for systems programming
  - How to use existing C libraries

- **[Zig's Relationship with C](https://andrewkelley.me/post/zig-cc-powerful-drop-in-replacement-gcc-clang.html)**
  - Understanding Zig as a C compiler
  - Cross-compilation benefits

## 🛠 Advanced Topics & Systems Programming

### OpenGL & Graphics Programming
- **[Zig OpenGL Bindings](https://github.com/hexops/mach-glfw)**
  - Modern OpenGL bindings for Zig
  - Part of the Mach game engine ecosystem

- **[Graphics Programming Examples](https://github.com/michal-z/zig-gamedev)**
  - Real-world graphics code in Zig
  - Useful for terminal emulator rendering

### Terminal & System Programming
- **[Zig Standard Library](https://ziglang.org/documentation/master/std/)**
  - `std.os` for system calls
  - `std.io` for terminal I/O
  - `std.Thread` for concurrency

- **[Terminal Programming Guide](https://viewsourcecode.org/snaptoken/kilo/)**
  - Not Zig-specific, but excellent terminal concepts
  - Great reference for QTerm development

### Build System
- **[Zig Build System](https://ziglearn.org/chapter-3/#zig-build-system)**
  - Understanding `build.zig`
  - Package management and dependencies

- **[Cross-compilation Guide](https://ziglearn.org/chapter-3/#cross-compilation)**
  - Zig's killer feature
  - Building for multiple targets

## 🎯 Project-Based Learning

### Small Projects to Build
1. **Command-line argument parser**
   - Practice structs and string handling
   - Foundation for QTerm CLI

2. **File watcher utility**
   - Learn async programming
   - System call usage

3. **Simple HTTP client**
   - Network programming
   - Error handling patterns

4. **Terminal color library**
   - ANSI escape code parsing
   - Directly useful for QTerm

### Inspiration Projects
- **[TigerBeetle](https://github.com/tigerbeetle/tigerbeetle)**
  - High-performance financial database in Zig
  - Excellent code quality examples

- **[Bun's Zig Code](https://github.com/oven-sh/bun)**
  - Real-world systems programming
  - Performance-critical code patterns

- **[River Window Manager](https://github.com/riverwm/river)**
  - Wayland compositor in Zig
  - Similar domain to QTerm (graphics/windowing)

## 🏠 Community & Support

### Official Channels
- **[Zig Discord](https://discord.gg/gxsFFjE)**
  - Very active and helpful community
  - `#help` channel for questions
  - `#learning` for learning discussions

- **[Zig Subreddit](https://www.reddit.com/r/Zig/)**
  - News, discussions, and questions
  - Weekly learning threads

- **[Zig Forums](https://ziggit.dev/)**
  - Official community forum
  - Long-form discussions

### Blogs & News
- **[Zig NEWS](https://zig.news/)**
  - Community articles and tutorials
  - Regular updates on ecosystem

- **[Loris Cro's Blog](https://kristoff.it/blog/)**
  - VP of Community at Zig Software Foundation
  - Deep insights into Zig design decisions

- **[Andrew Kelley's Blog](https://andrewkelley.me/)**
  - Creator of Zig
  - Design philosophy and development updates

## 🔧 Development Tools

### Editors & LSP
- **[zls (Zig Language Server)](https://github.com/zigtools/zls)**
  - Official language server
  - Works with VS Code, Vim, Emacs, etc.

- **[Zig VS Code Extension](https://marketplace.visualstudio.com/items?itemName=ziglang.vscode-zig)**
  - Syntax highlighting and IntelliSense
  - Integrated with zls

### Package Management
- **[Gyro](https://github.com/mattnite/gyro)** (Experimental)
  - Third-party package manager
  - Useful until official package manager arrives

- **[zig-package-template](https://github.com/mattnite/zig-package-template)**
  - Template for creating Zig packages
  - Best practices for project structure

## 📖 Quick Reference

### Essential Concepts (in order of learning)
1. **Basic syntax** (variables, functions, types)
2. **Error handling** (`!` and `try`)
3. **Memory management** (allocators, defer)
4. **Structs and enums**
5. **Optionals** (`?T`)
6. **Comptime basics**
7. **Testing** (built-in test framework)
8. **Build system** (`build.zig`)
9. **C interop** (`@import("c")`)
10. **Advanced comptime** (generics, reflection)

### Common Gotchas for C Developers
- No implicit conversions (use explicit casts)
- Arrays have compile-time known size
- Slices (`[]T`) vs arrays (`[N]T`)
- `undefined` is not zero (use explicit initialization)
- No function overloading (use generics instead)

### Performance Tips
- Prefer stack allocation when possible
- Use `comptime` to move work to compile time
- Profile before optimizing (use `zig build -Doptimize=ReleaseFast`)
- Understand different optimization modes

## 🎯 QTerm-Specific Resources

### Terminal Emulation
- **[VT100 User Guide](https://bitsavers.org/pdf/dec/terminal/vt100/EK-VT100-UG-001_VT100_User_Guide_Aug78.pdf)**
  - Classic terminal specification
  - Understanding ANSI escape sequences

- **[Terminal Emulator Development](https://nullprogram.com/blog/2017/10/06/)**
  - Excellent blog series on building terminals
  - C-focused but concepts apply to Zig

### Graphics & Font Rendering
- **[FreeType in Zig](https://github.com/hexops/mach-freetype)**
  - Zig bindings for font rendering
  - Essential for text display

- **[HarfBuzz Zig Bindings](https://github.com/hexops/mach-harfbuzz)**
  - Text shaping for ligatures
  - Part of modern text rendering pipeline

### Window Management
- **[Wayland Protocol Specs](https://wayland.freedesktop.org/docs/html/)**
  - Understanding Wayland protocols
  - Essential for Linux support

- **[X11 Programming with Zig](https://github.com/hexops/mach-x11)**
  - X11 bindings for traditional Linux setups

---

