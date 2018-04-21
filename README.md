# macOSX Setup with Ansible

- setup Xcode command line tools
`$ xcode-select --install`

- setup Homebrew
`$ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

- install git, ansible
`$ brew install git`
`$ brew install ansible`

- clone this repository
'$ git clone {{repository url}}`

- create `./user/main.yml` with medefying `./user/example`. fulfill your name and email for git

- Run ansible
`$ ansible-playbook site.yml -vvvv --ask-become-pass`

- Reboot
`$ sudo shutdown -r now`
