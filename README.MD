------------
### create_gui 主运行程序，创建GUI，生成用户图形界面
### OfficeAutomation 办公自动化集成功能文件
### img_process 图形文件处理为py文件，方便打包
### Img_source 处理后的图形py文件
------------
### 功能
- [x] Excel合并
  - [x] 同类型文件合并，有标题行
  - [ ] 支持文件合并是否取消第一行，即标题行；默认不合并第一行，作为标题行
  - [ ] 支持文件是否取消合并从标题行开始数任至任意行
  
- [x] pdf合并
  - [x] pdf文件合并 
  
- [x] 文件复制
  - [x] 根据提供的txt文件，内含文件名称部分信息
  - [x] 提供模糊搜索以及精确搜索，匹配成功后，将文件复制至新文件夹
  
- [x] 文件搜索
  - [x] 根据关键词搜索，文件内容若含有则输出绝对路径至文件
  - [ ] 多个关键词匹配
  - [ ] 文件搜索过程中，决定是否复制
  - [ ] 生成的目标列表文件位置在执行文件同级或复制后的路径位置
  - [ ] 支持添加单个关键词搜索
  
- [x] 文件比较
  - [x] 批量文件比较，两个文件夹有同样数量，同样名称的文件，移除相同文件，余下不同文件
  - [ ] 单个文件对比，添加弹窗信息表明异同

### GUI功能完善
- [x] 图标二值化处理
- [x] 背景添加
- [x] 重定向输出至debug.txt
  - [ ] 创建debug文件夹，文件存入其中（判断是否存在）
- [x] 打包
- [ ] License
- [ ] 日志模块
- [ ] 数据库(尚未想好应用场景)
- [ ] 缩小打包文件

### 打包错误
- [x] python gui打包,弹出缺少mkl_intel_thread.dll错误
* 解决方法：
* 复制以下dll文件至exe同级目录 libiomp5md.dll mkl_avx.dll mkl_avx2.dll mkl_avx512.dll mkl_core.dll mkl_intel_thread.dll mkl_p4.dll mkl_p4m.dll mkl_p4m3.dll mkl_rt.dll  mkl_sequential.dll mkl_tbb_thread.dll mkl_vml_avx.dll mkl_vml_avx2.dll mkl_vml_avx512.dll mkl_vml_cmpt.dll mkl_vml_ia.dll mkl_vml_p4.dll mkl_vml_p4m.dll mkl_vml_p4m2.dll mkl_vml_p4m3.dll
