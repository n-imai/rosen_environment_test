# rosen_environment_test

make environment  for test

## 構築手順

git clone https://github.com/n-imai/rosen_environment_test.git

cd rosen_environment_test

bundle install --path vendor/bundle

bundle exec berks vendor cookbooks

vagrant up

vagrant ssh-config --host hoge  >> ~/.ssh/config

bundle exec knife solo prepare hoge

bundle exec knife solo cook hoge
