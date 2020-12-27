# Live2D后端API

服务器状态监控系统：[筱锋服务器状态监控](https://status.lolicon.team/)

Docs构建文档：[Live2D](https://blog.2w2.top/doc-api/)

Live2D网页前端： [前端构建](https://github.com/ABSIDIA/live2d-widget/)
* * *

快速一键使用

```code
<script src="https://moeloli.club/live2d/autoload.js"></script>
```

### 接口调取方法

jsdelivr无法进行API调取，只能作为使用，如果需要调取请使用上方API服务，而不是jsdelivr服务

* 调用方法
    - /add/ **检测更新加缓存（正常勿需用到）**
    - /get/?id=X-Y **获取第X分组第Y号皮肤**
        - 其中分组为Live2d排列顺序
    - /rand/?id=X **根据上一个分组随即切换顺序**
    - /switch/?id=X **根据 上一分组 顺序切换**
    - /rand_textures/?id=X-Y **根据 上一皮肤 随机切换 同分组其他皮肤**
    - /switch_textures/?id=X-Y **根据 上一皮肤 顺序切换 同分组其他皮肤**

* 调用例子
    - /add/  **检测 新增皮肤 并更新 缓存列表**
    - /get/?id=1-23 **获取 分组 1 的 第 23 号 皮肤**
    - /rand/?id=1 **根据 上一分组 随机切换**
    - /switch/?id=1 **根据 上一分组 顺序切换**
    - /rand_textures/?id=1-23 **根据 上一皮肤 随机切换 同分组其他皮肤**
    - /switch_textures/?id=1-23 **根据 上一皮肤 顺序切换 同分组其他皮肤**

