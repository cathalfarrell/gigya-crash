source 'https://cdn.cocoapods.org/'

# Uncomment the next line to define a global platform for your project
platform :ios, '16.0'

use_frameworks!
#pods
def pods
  pod 'Gigya'
  pod 'GigyaTfa'
  pod 'GigyaAuth'
  pod 'GigyaNss'
end

target 'GigyaCrashOldSimulators' do
  pods
end


## Updating minimum deployment libraries to 16.0
post_install do |pi|
   pi.pods_project.targets.each do |t|
       t.build_configurations.each do |bc|
             bc.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '16.0'
           end
       end
  end
