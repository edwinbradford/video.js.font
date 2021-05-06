AV Neue Font.

The 'main' branch is an untouched mirror of the videojs/font 'master' branch and does not run on WSL Ubuntu. AV Neue Font development is in the 'avneue' branch which has been updated to work on WSL Ubuntu.

To get the 'avneue' branch working it was necessary to install GCC (Build Essentials) in Ubuntu for make, install Python2 in Ubuntu for Sass (Ubuntu 20.04.02 includes Python3), switch to Node 14.16.1 (LTS) in NVM (Node Version Manager), run npm update after npm install to fix multiple compile errors and uninstall then reinstall node-sass.

Package.json has been updated in the 'avneue' branch so grunt-cli and node-sass shouldn't require separate installation in future.

The steps to install were:

1. Install GCC (GNU Compiler Collection or Build Essential) in Ubuntu which will install make.
2. Install Python2 (legacy) in Ubuntu.
3. Use NVM (Node Version Manager) to switch to Node 14.16.1 (LTS).
4. Run $ npm install grunt-cli
5. Run $ npm install
6. Run $ npm update
7. Run $ grunt