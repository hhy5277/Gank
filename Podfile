source 'https://github.com/CocoaPods/Specs.git'
platform :ios, '10.0'
use_frameworks!

def pods
    pod 'XCGLogger'
    pod 'Alamofire', '~> 4.0'
    pod 'ReachabilitySwift'
    pod 'SwiftyJSON'
    pod 'Kingfisher','~> 3.1.0'
    pod 'FaceAware'
end

target 'Gank' do
    swift_version = '3.0'
    pods
end

post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['SWIFT_VERSION'] = '3.0'
        end
    end
end