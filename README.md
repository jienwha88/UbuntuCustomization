# UbuntuCustomization

first things to do
enabling workspace, changing the workspace size to be like OSX 1x4 (for now I just created 4)
gsettings set org.compiz.core:/org/compiz/profiles/unity/plugins/core/ vsize 1
gsettings set org.compiz.core:/org/compiz/profiles/unity/plugins/core/ hsize 4


Ubuntu Unity 16.04 
Setup gestures with fusuma:  
https://github.com/iberianpig/fusuma

Faced issues with installing fusuma, had to reinstall ruby: https://gorails.com/setup/ubuntu/16.04
Following these commands:  
The first step is to install some dependencies for Ruby.

sudo apt-get update
sudo apt-get install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev python-software-properties libffi-dev nodejs

```
cd
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
exec $SHELL

git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
exec $SHELL

rbenv install 2.4.1
rbenv global 2.4.1
ruby -v
 
```
modify gestures by creating ~/.config/fusuma directory, then creating config.yml

