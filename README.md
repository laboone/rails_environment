# 概要
ruby、mysqlが入ったubuntuのvagrantfile。
railsプロジェクトをすぐに始める用。
ansibleでプロビジョニングしているため、事前にansibleのインストールが必要。

# 始め方

```
$ brew install ansible
$ vagrant up
$ vagrant ssh
$ cd /vagrant && mkdir app && cd app
$ gem install rails
$ rails new . --database=mysql
$ rake db:create
# node入れない場合は、Gemfileの[gem 'therubyracer']のコメントを解除して以下を実行
$ bundle install
```
