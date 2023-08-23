source 'https://github.com/CocoaPods/Specs.git'

platform :ios, '12.0'

target 'GKDYVideo' do
  use_frameworks!

  pod 'AFNetworking'
  pod 'SDWebImage'
  pod 'SDWebImageWebPCoder'
  pod 'Masonry'
  pod 'YYModel'
  pod 'GKNavigationBar'
  pod 'GKVideoScrollView'
  pod 'GKPageSmoothView'
  pod 'GKSliderView'
  pod 'MJRefresh'
  pod 'JXCategoryView'
  
#  pod 'ZFPlayer'
  
  
  # 需要认证，不能免费使用了
  # pod 'TXLiteAVSDK_Player'  # 腾讯云播放器-独立播放器

end

post_install do |installer|
  # 消除版本警告
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      if config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'].to_f < 12.0
        config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '12.0'
      end
    end
  end
end
