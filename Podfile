# Uncomment this line to define a global platform for your project
platform :ios, '9.3'
# Uncomment this line if you're using Swift
use_frameworks!

target 'CardTrayDemo' do
	pod 'TesseractOCRiOS', '4.0.0'
end

target 'CardTray' do

end


target 'CardIOWrapper' do
    pod 'CardIO'
end

post_install do |installer|
    installer.pods_project.build_configuration_list.build_configurations.each do |configuration|
        configuration.build_settings['CLANG_ALLOW_NON_MODULAR_INCLUDES_IN_FRAMEWORK_MODULES'] = 'YES'
    end
end
