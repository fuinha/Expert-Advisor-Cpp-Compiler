# Expert-Advisor-Cpp-Compiler

This is a Nodejs package to help Fintechee's users compile C/C++ source codes(to make the expert advisors runnable on browser). It will be installed on your local PC. So, network is not required to compile your C/C++ source files.

To know more details about Fintechee, please access our official website: https://www.fintechee.com or our main Github repo: https://github.com/fintechee/Expert-Advisor-Studio

![Fintechee C/C++ compiler](https://github.com/fintechee/Expert-Advisor-Cpp-Compiler/blob/main/cpp.png)

## Prerequisite
Emscripten is required to compile C/C++ files.
So, you need to install it in advance.

## Usage
1. Installation

- Download the git repo, and then extract the zip file.
- cd the directory
- npm i

2. Run

- node app.js
- Access https://www.fintechee.com/web-trader/
- Click the "Console" on the menubar(on the left of the page).
- Choose "C/C++" tab on the panel.
- Open your C/C++ file and then click "Generate Indicator" or "Generate EA". C/C++ source codes and JSON will be generated. You can modify your original source codes by the generated codes. The generated parts are used to define the meta information of your program, such as the variables and data output and can be helpful to make your original codes compilable.
- Click "Compile Indicator" or "Compile EA" after you finish modifying your original codes.
- Use mql_indicator_loader_plugin or mql_ea_loader_plugin to load the compiled js(and Wenassembly).

3. Compiled files

- The compiled files will be stored in the sub-directory: ./static and you can access it via http://127.0.0.1:3000/js/[your_js_file_name]
- /js is the alias of ./static

## MIT
