# selfLearningRubyOnRails

sudo apt update
sudo apt upgrade

sudo apt install git g++ make vim libreadline-dev -y
sudo apt install libssl-dev zlib1g-dev nodejs -y

git clone https://github.com/rbenv/rbenv.git ~/.rbenv
echo 'export PATH="~/.rbenv/bin:$PATH"' >> ~/.profile
echo 'eval "$(rbenv init -)"' >> ~/.profile
. ~/.profile

git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build            
 
rbenv install -l
rbenv install 2.6.3
rbenv global 2.6.3
rbenv rehash
sudo apt install ruby-railties -y

gem install bundler
gem install rails -v 5.2.3 --no-document

sudo apt install postgresql
sudo apt install libpq-dev
sudo -u postgres createuser --createdb user

git --version
rbenv -v
ruby -v
bundler -v
rails -v
psql --version