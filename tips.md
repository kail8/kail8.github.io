## 踩坑记录

* 不需要本地下载Docker，只需要push到git远程仓库就行
* 配置自动编译：
    - Settings -> Actions -> General -> Workflow permissions -> Read and write permissions
    - Settings -> Pages -> source = "Deploy from a branch" & Branch = 'gh=pages'
* 修改navigation bar：在`_pages/*.md`中设置`nav: false`即可隐藏对应页面
    - `blog`标签页的开关应该在`_config.yml`中的`Blog`区块中的`pagination: false`