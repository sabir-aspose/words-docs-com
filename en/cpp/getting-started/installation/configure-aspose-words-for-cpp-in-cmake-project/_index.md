---
title: Configure the product in CMake Project
second_title: Aspose.Words for C++
articleTitle: Configure Aspose.Words for C++ in CMake Project
linktitle: Configure Aspose.Words for C++ in CMake Project
description: "Configure Aspose.Words for C++ in your CMake and build you application."
type: docs
weight: 90
ai_search_scope: words_cpp
ai_search_endpoint: "https://docsearch.api.aspose.cloud/ask"
ai_search_fast_endpoint: "https://docsearch.api.aspose.cloud/search"
url: /cpp/configure-aspose-words-for-cpp-in-cmake-project/
timestamp: 2024-10-24-11-44-28
---

Aspose.Words for C++ API works with CMake for any GNU/Linux operating system. It can be [downloaded from the official website](https://cmake.org/download/).

## Given CMake Project

Let's suppose you have the following CMake project:

*CMakeLists.txt:*
{{< highlight bash >}}
cmake_minimum_required(VERSION 3.18 FATAL_ERROR)
project(app CXX)
add_executable(app main.cpp)
{{< /highlight >}}

*main.cpp:*
{{< highlight bash >}}
int main()
{
    return 0;
}
{{< /highlight >}}

## Configure Manually

Follow the instructions below to manually configure Aspose.Words for C++ in your CMake:

1. [Download the latest Aspose.Words for C++ package](https://releases.aspose.com/words/cpp/)

2. Copy Aspose.Words.Cpp and `CodePorting.Native.Cs2Cpp_api_*.*` folders where you have CMakeLists.txt

3. Add the following lines to you CMakeLists.txt:
	{{< highlight cpp >}}
	# find Aspose.Words for C++ package and it's dependencies
	find_package(CodePorting.Native.Cs2Cpp REQUIRED CONFIG PATHS ${CMAKE_CURRENT_SOURCE_DIR} NO_DEFAULT_PATH)
	find_package(Aspose.Words.Cpp REQUIRED CONFIG PATHS ${CMAKE_CURRENT_SOURCE_DIR} NO_DEFAULT_PATH)
	find_package(Threads REQUIRED)

	# Link target application with Aspose.Words for C++
	target_link_libraries(app PRIVATE Aspose::Words Threads::Threads)
	{{< /highlight >}}

4. Now you can build you application using Aspose.Words for C++:
	{{< highlight bash >}}
	cd <path_to_dir_with_CMakeLists.txt>
	cmake -S . -B build -D CMAKE_BUILD_TYPE=Release
	cmake --build build
	./build/app
	{{< /highlight >}}

------ 

## FAQ

1. **Q:** How do I apply a license for Aspose.Words for C++?  
   **A:** After obtaining the `.lic` file, place it in a location accessible to your application and call `Aspose::Words::License license; license.SetLicense("path/to/Aspose.Words.Cpp.lic");` early in your code (e.g., at the start of `main`). This activates the full functionality without evaluation limitations.

2. **Q:** CMake reports “Could not find package Aspose.Words.Cpp”. What should I check?  
   **A:** Ensure the `Aspose.Words.Cpp` folder (containing the `Aspose.Words.CppConfig.cmake` file) is located in the same directory as your `CMakeLists.txt` or specify its path explicitly with `-D Aspose_Words_Cpp_DIR=/full/path/to/Aspose.Words.Cpp`. Also verify that you are using CMake 3.18 or newer.

3. **Q:** Can I install Aspose.Words for C++ in a custom directory and still use `find_package`?  
   **A:** Yes. After copying the package to a custom location, add the directory to `CMAKE_PREFIX_PATH` or pass it via the command line: `cmake -S . -B build -D CMAKE_PREFIX_PATH=/custom/path`. The `find_package` call will then locate the package.

4. **Q:** What is the minimum CMake version required for this configuration?  
   **A:** The example uses `cmake_minimum_required(VERSION 3.18)`. Versions prior to 3.18 lack proper support for the `CONFIG` mode used by Aspose.Words for C++ packages, so upgrade to at least 3.18.

5. **Q:** Do I need to link the `Threads` library on Windows as well?  
   **A:** Yes. The `Threads` component is required on all platforms. On Windows, CMake will resolve `Threads::Threads` to the appropriate system threading library, so the same `target_link_libraries` line works unchanged.