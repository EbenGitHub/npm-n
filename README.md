# npm-n
> Interactively Manage Your Node.js Versions
###
[npmjs-n](https://www.npmjs.com/package/n)
###
## Installation
> If you already have Node.js installed, an easy way to install `n` is using `npm`:
```bash
npm install -g n
```
or 
```bash
sudo npm install -g n
```
> If `npm` is not yet available, one way to bootstrap an install:
```bash
curl -L https://raw.githubusercontent.com/tj/n/master/bin/n -o n
bash n lts
# Now node and npm are available
npm install -g n
```
> On macOS with Homebrew you can install the n formula.
```bash
brew install n
```
> Or on macOS with MacPorts you can install the n port:
```bash
port install n
```
> On Linux and macOS, n-install allows installation directly from GitHub; for instance:
```bash
curl -L https://bit.ly/n-install | bash
```
###
## Installing Node.js Versions
> Simply execute n <version> to download and install a version of Node.js. If <version> has already been downloaded, n will install from its cache.
```bash
n 10.16.0
n lts
```
or
```bash
sudo n 10.16.0
sudo n lts
```
> If "node --version" shows the old version then start a new shell, or reset the location hash with:
```bash
hash -r
```
or
```bash
rehash
```
###
## Removing Versions
> Remove some cached versions:
```bash
n rm 0.9.4 v0.10.0
```
> Removing all cached versions except the installed version:
```bash
n prune
```
> Remove the installed Node.js (does not affect the cached versions). This can be useful to revert to the system version of node (if in a different location), or if you no longer wish to use node and npm, or are switching to a different way of managing them.
```bash
n uninstall
```
