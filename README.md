# uniapp
uniapp+uview h5版本 也可以编译其他版本.
###########
路由获取参数在onLoad里面 加载会获取options参数 onLoad(options){}
#1.1 路由参数params里面不能出现对象 要转换成字符串传过去 
#2.小程序不存在跨域 必须https 401 403 405 都是少参数
#3.imgBase.replace(/[\r\n]/g,"") base64编码显示图片base64自动换行bug 
#4.路由跳转 uni.$u.route()
#5.图片动态路径需要 require('@/static....') 或者静态路径，图片名字必须英文（安卓中文不显示）
#6 v-show无效 要换成 v-if
#7 u-picker 组件报错 需要修改里面city areas值为空
#8 u-form-item 添加props target验证， 表单循环校验可以直接添加 :target='item' 
#9 uview自带校验必须是字符串 不然会通过不了 
#10 小程序路由跳转超过10次就会无效navigateTo  部分路由修改reLaunch以及redirectTo
#发布流程
#1.开发者工具上传代码，如果代码太大要进行代码优化，分包加载，图片压缩 官方文档有步骤

