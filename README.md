# go-app-package

How to package golang app with dh-make-golang and dh-golang.

## Dependencies

In ubuntu, please use the below command to install packaginge compile
dependencies:

    $ sudo apt install dh-make-golang dh-golang

## How to packaging

You should first create a golang app repo in [github.com/mutse/go-app-package](https://github.com/mutse/go-app-package)

Generate debian package with dh-make-golang command:

    $ dh-make-golang github.com/mutse/go-app-package
    $ sendmail -t < itp-go-app-package.txt
    $ cd go-app-package
    $ debuild
