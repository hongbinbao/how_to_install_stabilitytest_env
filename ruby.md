ruby on ubuntu 14.04 64bit
1: rvm
    curl -L https://get.rvm.io | bash -s stable
  
2: active rvm
    source ~/.rvm/scripts/rvm

3: verify rvm version
    rvm -v

4: install ruby version 1.9.3
    rvm install 1.9.3
    
5: set ruby 1.9.3 as system default
    rvm 1.9.3 --default

6: Ruby Gem package manager for installing Ruby packages.(since 1.9.2)
    gem -v
    
7: install Ruby packages: sass
    gem install sass
    gem install compass

8: switch Gem source
    gem source -r https://rubygems.org/
    gem source -a https://ruby.taobao.org
