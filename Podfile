platform :ios, '9.0'
inhibit_all_warnings!

def shared_pods
    pod 'SwiftLint'
    pod 'MagicalRecord'
    pod 'SkyFloatingLabelTextField', '~> 3.0'
    pod 'RSKImageCropper'
    pod 'MaterialComponents/Tabs'
    pod 'DLRadioButton', '~> 1.4'
    pod 'Fabric'
    pod 'Crashlytics'
    pod 'SwiftyBeaver'
    pod 'SnapKit', '~> 4.0.0'
    pod 'UITextView+Placeholder', '~> 1.2'
    pod 'OneSignal', '>= 2.6.2', '< 3.0'
    pod 'OpenTok'
    pod 'FSUtils'
    pod 'LUExpandableTableView'
    pod 'MBProgressHUD', '~> 1.1.0'
    pod 'lottie-ios'
    pod 'Cosmos', '~> 15.0'
    pod 'IQKeyboardManager', :inhibit_warnings => true
    pod 'SwiftyJSON'
    pod 'Stripe'
    pod 'AFNetworking', '~> 3.0.0'
    pod 'SwiftValidators'
    pod 'Alamofire'
    pod 'Kingfisher'
    pod 'SACodedTextField'
end

target 'Test' do
    use_frameworks!
    shared_pods
end

post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['CONFIGURATION_BUILD_DIR'] = '$PODS_CONFIGURATION_BUILD_DIR'
            config.build_settings['CLANG_WARN_DOCUMENTATION_COMMENTS'] = 'NO'
        end
    end
end
