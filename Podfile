# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'Udong' do
pod 'KakaoSDKCommon'  # 필수 요소를 담은 공통 모듈
pod 'KakaoSDKAuth'  # 사용자 인증
pod 'KakaoSDKUser'  # 카카오 로그인, 사용자 관리
pod 'SnapKit', '~> 5.0.0'
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings["ONLY_ACTIVE_ARCH"] = "NO"
    end
  end
end
