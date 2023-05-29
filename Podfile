platform :ios, '12.1'

target 'Love In A Snap' do
  use_frameworks!

  pod 'TesseractOCRiOS'
  pod 'GPUImage'

end

post_install do |installer|
    installer.generated_projects.each do |project|
          project.targets.each do |target|
              target.build_configurations.each do |config|
                  config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '13.0'
               end
          end
   end
end
