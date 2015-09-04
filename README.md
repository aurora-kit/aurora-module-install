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

  Removing this reference, the installer will `init` the repository in case you pass the url when run the script. 
  You could always download the files directly and won't have to remove this reference.

3. Launch the installer

  ```
    $ ./install
  ```

  Probably you'll need to `chmod +x install`


### Dependencies
To be able to manipulate the `package.json` file with the variables you passed, it's necessary to have [jq](https://stedolan.github.io/jq/) installed.

### What this script do
After ask you some fast information about the module/folder (keep in mind that most have a default value):

- Add the title and description to a `README.md` file
- Create a `src` directory (or the name you choose)
- Create the component files inisde the `src` folder
- Create the main file in the same folder with the code to `@import` the partials files
- [optional] Create a debug file that `@import` the necessary assets
- Update `name`, `description`, `repository` urls on `package.json` file
- [optional] Add `gulpfile.js`, `.gitignore` and other dot files
- [optional] Initialize git repository
- [optional] Install the `npm` packages
- [optional] Delete the install files


---
[MIT license](http://opensource.org/licenses/MIT)
