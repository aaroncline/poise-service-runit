#
# Copyright 2015, Noah Kantrowitz
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
# http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#

source 'https://rubygems.org/'

gemspec path: File.expand_path('..', __FILE__)

gem 'halite', path: '../halite'
gem 'poise', path: '../poise'
gem 'poise-service', path: '../poise-service'
# gem 'halite', github: 'coderanger/halite'
# gem 'poise', github: 'poise/poise'
# gem 'poise-service', github: 'poise/poise-service'

group :development do
  gem 'rake', '~> 10.4.2'
  gem 'pry'
  gem 'travis'
end

group :test do
  gem 'rspec', '~> 3.1.0'
  gem 'rspec-its', '~> 1.1.0'
  gem 'chefspec', '~> 4.2.0'
  gem 'fuubar', '~> 2.0.0'
  gem 'simplecov', '~> 0.9.1'
  gem 'foodcritic'
end

group :integration do
  gem 'test-kitchen', '~> 1.3.1'
  gem 'kitchen-vagrant'
  gem 'vagrant-wrapper'
  gem 'kitchen-docker'
  gem 'kitchen-sync'
  gem 'berkshelf'
end

group :travis do
  gem 'codeclimate-test-reporter'
end
