# This file manages Puppet module dependencies.
#
# It works a lot like Bundler. We provide some core modules by
# default. This ensures at least the ability to construct a basic
# environment.

def github(name, version, options = nil)
  options ||= {}
  options[:repo] ||= "boxen/puppet-#{name}"
  mod name, version, :github_tarball => options[:repo]
end

# Includes many of our custom types and providers, as well as global
# config. Required.

github "boxen", "1.2.0"

# Core modules for a basic development environment. You can replace
# some/most of these if you want, but it's not recommended.

github "dnsmasq",   "1.0.0"
github "gcc",       "1.0.0"
github "git",       "1.0.0"
github "homebrew",  "1.1.2"
github "hub",       "1.0.0"
github "inifile",   "0.9.0", :repo => "cprice-puppet/puppetlabs-inifile"
github "nginx",     "1.1.0"
github "nodejs",    "1.0.0"
github "nvm",       "1.0.0"
github "ruby",      "3.1.0"
github "stdlib",    "3.0.0", :repo => "puppetlabs/puppetlabs-stdlib"
github "sudo",      "1.0.0"

# Optional/custom modules. There are tons available at
# https://github.com/boxen.

github "mongodb",   "1.0.0"
github "hipchat",   "1.0.2"
github "skype",     "1.0.2"
github "firefox",   "1.0.3"
github "chrome",    "1.0.0"
github "wget",      "1.0.0"
github "phantomjs", "1.0.0"
github "virtualbox","1.0.1"
github "vagrant",   "1.0.1"
github "iterm2",    "1.0.1"
github "java",      "1.0.6"
github "textmate",  "1.1.0"
github "alfred",    "1.0.1"
github "dropbox",   "1.1.0"
github "1password", "1.0.0", :repo => "payperks/puppet-1password"
github "pycharm",   "1.0.2", :repo => "payperks/puppet-pycharm"

# fun stuff [modules here won't be installed globally, these are per user. ]
# check https://github.com/boxen/our-boxen/blob/master/modules/people/README.md

github "adium",   "1.0.1"
github "rdio",    "1.0.0"

