# Aurora module installe
A bash script to automate the initial stuff for new `css` modules.

### Install
1. Clone this repo

  ```
    $ git clone https://github.com/aurora-kit/aurora-module-install myNewModule
  ```

2. Remove the `.git` reference

  ```
    $ rm -rf .git
  ```

  Removeing this reference, the installer will `init` the repository in case you'll pass the url. 
  You could always download the files directly and won't have to remove this reference.

3. Launch the installe

  ```
    $ ./install
  ```

  Probably you'll need to `chmod +x install`