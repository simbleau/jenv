# jenv
jenv (Java Environment) is a minimalist CLI bash tool to manage a java project source and binary structure for easy debugging.

## Synopsis:
jenv will orchestrate your classpath and handle source compiling to make it 
easier to debug Java programs spanning several packages. To use jenv, every
single Java project you create must follow a conventional hierarchy. This is 
because I insist that every Java project be handled properly and conventionally.

## Project Structure
The structure you must obey is as follow:
...\
.../root_dir/			Root Directory\
.../root_dir/src/		Source Directory\
.../root_dir/bin/		Classpath(Binary) Directory\
\
Essentially, every project folder must have a 'src' (source) folder and a 'bin'
(binary) export folder. The bin folder will be where java class files are 
generated on compilation, and the src folder is where java source files must 
exist to be compiled. It's that simple.

## Usage
"jsrc <src_dir>" will set the source directory for the java environment.\
"jcomp" will compile your java source files into the bin directory.\
"jenv" will print the current java environment details. Use this to double check your environment.
