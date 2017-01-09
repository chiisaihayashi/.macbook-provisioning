# my macbook provisioning

##setup homebrew
```
$ sudo xcodebuild -license
$ xcode-select --install
$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

##install pre-req
```
$ brew install python
$ brew install ansible
$ brew install caskroom/cask/brew-cask
```

##cloning ansible repo
```
$ git clone https://github.com/chiisaihayashi/.macbook-provisioning
```

##provisioning
```
$ cd .macbook-provisioning/
$ ansible-playbook -i hosts -vv localhost.yml
```

##post
```
$ sudo vi /etc/shells
$ chsh -s /usr/local/bin/zsh
```
