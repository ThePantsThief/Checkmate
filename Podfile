platform :ios, '9.0'

inhibit_all_warnings!

target 'Checkmate' do
  pod 'Objc-iOS-Extensions' => '0.1.0'
  pod 'TBAlertController'
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '9.2'
    end
  end
end