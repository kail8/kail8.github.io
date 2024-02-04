## 踩坑记录

* 不需要本地下载Docker，只需要push到git远程仓库就行
* 配置自动编译：
    - Settings -> Actions -> General -> Workflow permissions -> Read and write permissions
    - Settings -> Pages -> source = "Deploy from a branch" & Branch = 'gh=pages'
* 修改navigation bar：在`_pages/*.md`中设置`nav: false`即可隐藏对应页面
    - `blog`标签页的开关应该在`_config.yml`中的`blog_nav_title: `设为空
* 配置bib-author：
    - 在`_config.yml`修改对应的`scholar.first_name`和`scholar.last_name`即可加粗自己的名字
* 配置页面样式:
    - `_sass/_base.scss`给主页面的联系方式`social`添加padding (修改margin无效)
* 添加访客统计：
    - 在[clustrmaps](https://clustrmaps.com/)里面申请账号，然后把js代码插入到`_layout/about.html`的`social` div 下面，但要用一个div包起来，然后在`_scss/_base.scss`给`clustrmaps-container`设置宽度