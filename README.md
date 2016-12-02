# 1.PrivateSpecs
PrivateSpecs是个人cocoapods私库搭建的ios私有仓库
# 2. 使用说明
- 封装ios控件（或者模块）
- 编写PodSpec文件
- 检查和验证PodSpec的合法性

  >pod lib lint --sources='https://github.com/liuzewen/PrivateSpecs.git'
- 将封装好的控件（或者模块）打上tag标签

   >git tag -m "release" "0.0.1"
   
   >git push --tags    

- 将封装的控件（或者模块）上传至PrivateSpecs


  >pod repo push 'PrivateSpecs' 项目名.podspec

# 3.项目引用说明
在Podfile文件中添加一下内容：

source 'https://github.com/liuzewen/PrivateSpecs.git' 
source 'https://github.com/CocoaPods/Specs.git'  

