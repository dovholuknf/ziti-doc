# Building this Project

## Prerequisite

* [docfx](https://dotnet.github.io/docfx/) needs to be on your path
* Linux - Documentation is run routinely by our CI
* Windows - Developed with [Windows Subsytem for Linux (WSL)](https://docs.microsoft.com/en-us/windows/wsl/install-win10)
* Doxygen - [Doxygen](http://www.doxygen.nl/) is used to generate the api documentation for the C SDK and is
  necessary to be on the path
  
## Building the Doc

Github offers [github pages](https://pages.github.com/) which this project uses to host the output of building the
static content. Github has a few options for where you can put your doc at this time, the master branch, a folder on the
master branch named 'docs' or a special branch that still works named "gh-pages". This project is currently configured
to use the master branch and docs folder.

The best/easiest thing to do in order to build these docs is to have Windows Subsytem for Linux installed or any shell
which can execute a `.sh` script. As of 2020 there's a multitude of ways to get a bash/shell interpreter in windows.
It's not feasible to test all these shells to make sure this script works so it's encouraged that you use a linux-based
flavor of bash. If the script doesn't funtion - open an [issue](./issues) and someone will look into it.

After cloning this repository open the bash shell and execute the [](build-doc.sh) script.
