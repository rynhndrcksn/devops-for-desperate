# Devops for the Desperate
Repo that goes along with the [DevOps for the Desperate](https://nostarch.com/devops-desperate) book.

## About
DevOps for the Desperate is a book by Bradley Smith that provides an introduction to DevOps, CI/CD, Vagrant, Ansible, Docker, and Kubernetes.

## Installation
As I'm using a M1 MacBook Pro, there's some special setup required. Bradley Smith did their best to help in the book with people using M1 Macs, but I ran into way more problems than the book could solve.
1. Install [HomeBrew](https://brew.sh) `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`.
2. Install [Vagrant](https://www.vagrantup.com/) `brew install --cask vagrant`.
3. Install [Vagrant VMWare Utility](https://www.vagrantup.com/vmware/downloads) `brew install --cask vagrant-vmware-utility`.
4. Install VMWare Fusion provider `vagrant plugin install vagrant-vmware-desktop`.
5. Install [VMware Fusion Technology Preview 21H1 (for ARM)](https://customerconnect.vmware.com/downloads/get-download?downloadGroup=FUS-PUBTP-2021H1).
6. Because of the Vagrant VMWare Utility not liking the VMWare Fusion tech preview, we need to create a symlink `ln -s "/Applications/VMware Fusion Tech Preview.app" "/Applications/VMware Fusion.app"` and this works because the Vagrant VMWare Utility is written in Go and works with Rosetta 2 just fine.

## Contributing
Pull requests are not accepted right now, due to this being a repo containing the files I'm using to learn DevOps.

## License
This project uses an [MIT](https://opensource.org/licenses/MIT) license that you can find [here](LICENSE).

https://customerconnect.vmware.com/downloads/get-download?downloadGroup=FUS-PUBTP-2021H1