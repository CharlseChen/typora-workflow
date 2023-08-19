# typora-workflow
使用传入文件名，快捷新建一个markdown文件
## 前提
+ 需要本地安装一个typora应用
+ 亦或者安装别的markdown编辑器
## 安装
+ 下载md.alfredworkflow文件后，双击后按alfred提示安装即可
## 配置
+ 进入下面界面，双击下方红色框中组件
  <img width="771" alt="image" src="https://github.com/CharlseChen/typora-workflow/assets/13670267/a1a90d52-8139-4c71-a11b-065052ebcaf8">

+ 编辑markdown文件默认保存路径
  <img width="771" alt="image" src="https://github.com/CharlseChen/typora-workflow/assets/13670267/a342c9ff-6221-461b-9d83-fc0be8ae7f00">
+ 点击保存（“save”）
+ 最后，重载插件即可
  
  <img width="503" alt="image" src="https://github.com/CharlseChen/typora-workflow/assets/13670267/03784fe2-3696-4012-9d45-7a3f9977a2b3">

### PS:上面的工作流插件脚本亦可以用于创建其他类型的文件，脚本文件如下
```
# 获取输入参数（文件名包括后缀）
filename=$1

# Markdown 文件路径
file_path="/Users/chenhao/Desktop/$filename"

touch "$file_path"
open -a "Typora" "$file_path" #这里的Typora换成你需要创建文件类型对应的编辑器，例如Sumlime
```
