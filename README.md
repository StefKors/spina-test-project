# Setup instructions
1) run `rails new spina_example --database postgresql` Create a new rails app
2) run `cd spina_example`
3) run `rails db:create`
   1) run `brew services start postgresql` (if postgresql is not running)
4) run `rails active_storage:install`
5) add `gem 'spina'` to bottom of the `Gemfile`
6) run `bundle install`
7) run `rails g spina:install`
   1) answer questions
8) run `rails s`
9) login at `http://localhost:3000/admin`

removed this line in the application haml file:
= javascript_include_tag 'application', 'data-turbolinks-track' => true