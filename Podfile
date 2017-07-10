# Uncomment this line to define a global platform for your project
platform :ios, '10.0'
use_frameworks!

target 'Starter-Project' do
    
    pod 'Material', '~> 2.0'
    pod 'SwiftyJSON'
    pod 'Alamofire', '~> 4.0'
    pod 'SwiftLint'
    pod 'SwiftIconFont'
    pod 'Kingfisher', '~> 3.0'
    pod 'Motion', '~> 1.0'
    pod 'PromiseKit', '~> 4.0'
    pod 'Fabric'
    pod 'Crashlytics'
    pod 'Answers'
end

post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['SWIFT_VERSION'] = '3.0'
        end
    end
end
