# coding: utf-8

#
# セットアップ用のタスク
#
task :setup => %w[
     setup:gem
     setup:pods
]

namespace :setup do
  desc "Gem をインストールする"
  task :gem do
    sh "bundle -j4 --path vendor/bundle"
  end

  desc "Pods をインストールする"
  task :pods do
    sh "bundle exec pod install"
  end
end
