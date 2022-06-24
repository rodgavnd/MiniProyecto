# Mini proyecto 

## SetUp
```sh
#terminal
ruby --v
sudo  gem install bundler
bundler -v
touch Gemfile
open Gemfile 
    source "https://rubygems.org"
    gem "cocoapods", '1.10.0'
bundle install
pod --version
pod init
open Podfile
# ejecutar bundle si quiere que lo haga con la version de ruby seteada
bundle exec pod install 
# ejecutar si no quiere utilizar la version de ruby seteada
pod install
```

## enable rosetta
    1. open finder->Aplications
    2. search terminal->left clic->get information->check open with rosetta
    2. search xcode->left clic->get information->check open with rosetta
    
## add Google Maps in Podfile
```sh
source 'https://github.com/CocoaPods/Specs.git'

platform :ios, '12.0'

target 'YOUR_APPLICATION_TARGET_NAME_HERE' do
  pod 'GoogleMaps', '6.2.1'
end
pod install

# if pod install fail
sudo arch -x86_64 gem install ffi
arch -x86_64 pod install 
#or
pod install
```
