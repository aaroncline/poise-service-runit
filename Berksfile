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

source 'https://supermarket.chef.io/'
extension 'halite'

# Force the rebuild every time for development.
cookbook 'poise', gem: 'poise'
cookbook 'poise-service', gem: 'poise-service'
cookbook 'poise-service-runit', gem: 'poise-service-runit'

group :test do
  cookbook 'poise-service-runit_test', path: 'test/cookbooks/poise-service-runit_test'
  cookbook 'apt'
end

# For the master build, pull in the runit cookbook from git.
if ENV['POISE_MASTER_BUILD']
  cookbook 'runit', github: 'hw-cookbooks/runit', branch: 'develop'
end
