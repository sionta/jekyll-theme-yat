# frozen_string_literal: true

source "https://rubygems.org"
gemspec

platforms :mingw, :x64_mingw, :mswin, :jruby do
  # Windows and JRuby does not include zoneinfo files, so bundle the tzinfo-data gem
  # and associated library.
  gem "tzinfo", "~> 2.0.6"
  gem "tzinfo-data", "~> 1.2024.1"

  # Performance-booster for watching directories on Windows
  gem "wdm", "~> 0.1.1"

  # Lock `http_parser.rb` gem to `v0.6.x` on JRuby builds since newer versions of the gem
  # do not have a Java counterpart.
  gem "http_parser.rb", "~> 0.8.0"
end
