Install guide for Ubuntu (20.04.2 LTS).

To get Videojs Font working it was necessary to install GCC (Build Essentials) in Ubuntu for make, install Python2 in Ubuntu for Sass (Ubuntu 20.04.02 includes Python3), use Node 14.16.1 (LTS) in NVM (Node Version Manager), run npm update after npm install to fix multiple compile errors then uninstall and reinstall node-sass.

Package.json has been updated in this fork to include working versions of grunt-cli and node-sass in devDependencies so hopefully they no longer require separate installation.

1. Install GCC (GNU Compiler Collection or Build Essential) in Ubuntu which will install make.
2. Install Python2 (legacy) in Ubuntu.
3. Use NVM (Node Version Manager) to switch to Node 14.16.1 (LTS).
4. Run $ npm install grunt-cli
5. Run $ npm install
6. Run $ npm update
7. Run $ grunt