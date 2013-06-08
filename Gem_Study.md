gem list
-----------

# coding: utf-8
* source 'http://ruby.taobao.org'

* gem "rails", "4.0.0.rc1"  http://edgeguides.rubyonrails.org/
* gem 'actionpack-action_caching', '1.0.0' https://github.com/rails/actionpack-action_caching
* gem 'sass-rails', "~> 4.0.0.rc1"  https://github.com/rails/sass-rails
* gem 'coffee-rails', "~> 4.0.0" https://github.com/spastorino/coffee-rails
* gem 'uglifier', '>= 1.3.0' https://github.com/lautis/uglifier

* gem "rails-i18n","0.1.8" https://github.com/svenfuchs/rails-i18n
* gem "jquery-rails", "2.0.1"  https://github.com/rails/jquery-rails
* gem "rails_autolink", ">= 1.1.0" https://github.com/tenderlove/rails_autolink
* gem "jquery-atwho-rails", "0.1.6"  https://github.com/ichord/jquery-atwho-rails
* gem "md_emoji" https://github.com/elm-city-craftworks/md_emoji
* gem 'exception_notification' https://github.com/rails/exception_notification

# 上传组件
* gem 'carrierwave', '0.6.2' https://github.com/carrierwaveuploader/carrierwave
* gem 'carrierwave-upyun', '0.1.5' https://github.com/nowa/carrierwave-upyun
* gem 'mini_magick','3.3', require: false https://github.com/probablycorey/mini_magick

# Mongoid 辅助插件
* gem "mongoid", github: 'mongoid/mongoid', ref: '11e45e5a30a45458b83db99ab6c9d9ccc337e66f' https://github.com/mongoid/mongoid
* gem 'mongoid_auto_increment_id', "0.6.1" https://github.com/huacnlee/mongoid_auto_increment_id
* gem 'mongoid_rails_migrations', '1.0.0' https://github.com/adacosta/mongoid_rails_migrations

# 用户系统
* gem 'devise', '3.0.0.rc' https://github.com/plataformatec/devise
* gem 'devise-encryptable', '0.1.2' https://github.com/plataformatec/devise-encryptable

# 分页
* gem 'will_paginate', '3.0.4' https://github.com/mislav/will_paginate

# Bootstrap
* gem 'anjlab-bootstrap-rails', '2.0.3.2', require: 'bootstrap-rails' https://github.com/anjlab/bootstrap-rails
* gem 'bootstrap-will_paginate', '0.0.3' https://github.com/yrgoldteeth/bootstrap-will_paginate
* gem 'bootstrap_helper', "4.2.2.2"  https://github.com/xdite/bootstrap-helper

# 三方平台 OAuth 验证登陆
* gem "omniauth", "~> 1.0.1" https://github.com/intridea/omniauth
* gem "omniauth-github", "~> 1.1.0" https://github.com/intridea/omniauth-github

# permission
* gem "cancan", "~> 1.6.10" https://github.com/ryanb/cancan

# Redis 命名空间
* gem 'redis-namespace','~> 1.2.1' https://github.com/resque/redis-namespace

# 将一些数据存放入 Redis
* gem "redis-objects", "0.5.2" https://github.com/nateware/redis-objects

# Markdown 格式
* gem "redcarpet", "~> 2.2.2" https://github.com/vmg/redcarpet
* gem "rouge", "~> 0.3.2" https://github.com/jayferd/rouge
* gem 'nokogiri', "~> 1.5.6" https://github.com/sparklemotion/nokogiri

# YAML 配置信息
* gem "settingslogic", "~> 2.0.9" https://github.com/binarylogic/settingslogic

* gem "cells", github: 'apotonick/cells', ref: '0dcdc190e949af1a821f31f33f76f407a6da47b4' https://github.com/apotonick/cells

# 队列
* gem "sidekiq", "2.5.3" https://github.com/mperham/sidekiq

* gem 'faye-rails','1.0.0' https://github.com/jamesotron/faye-rails

# 分享功能
* gem "social-share-button", '0.1.4' https://github.com/huacnlee/social-share-button

# 表单
* gem 'simple_form', "3.0.0.rc" https://github.com/plataformatec/simple_form

# API
* gem 'grape', github: 'intridea/grape', branch: 'frontier' https://github.com/intridea/grape

# Mailer
* gem 'postmark-rails', '0.4.1' https://github.com/wildbit/postmark-rails

# Google Analytics performance
* gem 'garelic', '0.0.2' https://github.com/jsuchal/garelic

* gem "god" https://github.com/mojombo/god

* gem 'dalli', '1.1.1' https://github.com/mperham/dalli

group :development, :test do
  * gem 'capistrano', '2.9.0', require: false https://github.com/halorgium/capistrano
  * gem 'rvm-capistrano', require: false https://github.com/wayneeseguin/rvm-capistrano
  * gem 'rspec-rails', '~> 2.13.2' https://github.com/rspec/rspec-rails
  * gem 'factory_girl_rails' https://github.com/thoughtbot/factory_girl_rails
  * gem 'database_cleaner' https://github.com/bmabey/database_cleaner
  * gem "rspec-cells", '0.1.7' https://github.com/kpumuk/rspec-cells
  * gem "capybara", "~> 0.4.1" https://github.com/jnicklas/capybara
  * gem 'api_taster', '0.6.0' https://github.com/fredwu/api_taster
  * gem "letter_opener" https://github.com/ryanb/letter_opener
  * gem 'thin', "1.5.0"  https://github.com/macournoyer/thin

  # 用于组合小图片
  * gem "sprite-factory", "1.4.1", require: false https://github.com/jakesgordon/sprite-factory
  * gem 'chunky_png', "1.2.5", require: false https://github.com/wvanbergen/chunky_png

  * gem 'jasmine', '1.2.1' https://github.com/pivotal/jasmine
  * gem "mongoid_colored_logger", "0.2.2"  https://github.com/romanbsd/mongoid_colored_logger
  
  * gem "quiet_assets", "~> 1.0.2" https://github.com/evrone/quiet_assets
end

group :production do
  * gem 'unicorn' https://github.com/defunkt/unicorn
  * gem 'newrelic_rpm' https://github.com/smtlaissezfaire/newrelic_rpm
end
