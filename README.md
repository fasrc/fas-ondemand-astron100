# Remote Desktop environment for class ASTRON 100
based on original [OSC bc_desktop](https://github.com/OSC/bc_desktop) by OpenOnDemand developers 

This application provides an environment for class Astron100, with icons to start Anaconda navigator, spyder and Visual Studio Code.

currently points at a centos 7 container which includes:
   - VSCode 1.47.3
   - Anaconda 

Other applications can be loaded from command line from the modules system as described on our [documentation page](https://docs.rc.fas.harvard.edu/kb/modules-intro/)

## Install

The master branch of this repo is automatically deployed by puppet to /var/www/ood/apps/sys/ on the ondemand nodes.

If you want to deploy that in your user development environment to make modifications, follow these instructions.

```sh
# create the development folder if you still not have one
mkdir -pv $HOME/fasrc/dev/
cd $HOME/fasrc/dev/

# clone the repository in a subfolder for your version of the app
git clone https://github.com/fasrc/fas-ondemand-astron100.git

# Change the working directory to this new directory
cd fas-ondemand-astron100
```
You can now make your preferred modifications and run your version of the app from the sandbox control panel under the
*dev* menu on the ondemand dashboard

## Contributing

If you intend deploy your modified version as system wide app, please commit your changes to a branch first, and open a PR.

