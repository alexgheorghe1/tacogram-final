source "https://rubygems.org"
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby "2.7.5"

gem "rails", "~> 7.0.2.2"
gem "puma", "~> 5.0"
gem "bcrypt", "~> 3.1.7"
gem "tzinfo-data", platforms: %i[ mingw mswin x64_mingw jruby ]
gem "image_processing", ">= 1.2" #links out to internet and pulls into application
gem "aws-sdk-s3", require: false #talks to AWS external service; library that talks to AWS API endpoint

group :development, :test do
  gem "debug", platforms: %i[ mri mingw x64_mingw ]
end

group :development do
  gem "sqlite3", "~> 1.4"
  gem "tabulo"
  gem "web-console"
end

group :production do
  gem "pg" #enterprise level sql that works with heroku
end