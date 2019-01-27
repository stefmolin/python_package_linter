# Python Package Linter
Bash script for running `pylint` on a package and breaking the outputs into a cleaner format.

## Requirements
You will need to install `pylint` and be sure to tailor the `.pylintrc` file to your needs. 

## Usage
1. Place this file at the same level as the top level folder of your package. 
2. On line 12 of the `lint_package` file, provide the name of your package as it appears in the file system.
3. Run `./lint_package` from the command line (adjust path as needed based on your `pwd`).

*Note, if you wish to use a `.pylintrc` file that is named otherwise, specify it on line 11.*

## Output
The script will provide you with dependency graphs between the subpackages and modules of your package, as well as, with outside packages. The potential issues `pylint` finds with each module will be broken out into separate files in the same file structure as the package itself in the `reports_by_module` directory. 

Once the script finishes, it will tell you exactly where the files will be.
