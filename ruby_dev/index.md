# Ruby Development

## Command Line Parser

Using gem main

## Bundler

Q:How to using script outside the project directory
A:bundler code needs to know Gemfile to do it work. Default, it will search current directory. However, if you want exec script without Gemfile in current directory and with bundle prefix command, please do following:

ruby{{{
ENV['BUNDLE_GEMFILE']=File.dirname( File.realpath( __FILE__ ) ) + "/../Gemfile"

require 'bundler/setup'
}}}

This code will specify BUNDLE_GEMFILE and load bunder code.


