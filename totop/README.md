# Docsify toTop

Docsify 返回顶部实现方式，源代码来自 https://github.com/mmkjony/jQuery.toTop ，遵循 MIT 许可证。
## Demo

## 使用
**1. 根据 Docsify [官方文档](https://docsify.js.org/#/)新建一个项目。**

**2. 项目中新建一个 `js` 文件夹，将 [jquery.toTop.min.js](https://github.com/injellyfish/docsify-toTop/blob/main/jquery.toTop.min.js) 加入到文件夹中。**

**3. 复制以下代码到项目的 `index.html` 中。**
```html
<a class="to-top">Top &uarr;</a>
<script src="https://cdn.staticfile.org/jquery/1.12.4/jquery.min.js"></script>
<script src="/js/jquery.toTop.min.js"></script>
<script>
  $('.to-top').toTop({
      //options with default values
      autohide: true,
      offset: 420,
      speed: 500,
      position: true,
      right: 15,
      bottom: 30
  });
</script>
```
## 自定义
您可以通过修改 `<a class="to-top">Top &uarr;</a>` 进行自定义。

另外，根据源代码作者的注释，可以进行以下修改：

| Option        | Value           | Desciption  |
| :------------- |:-------------| :-----|
| autohide | boolean | You have options whether you want your button to hide automatically or not. You can choose 'true' or 'false'. `default: true` |
| offset | Integer (px) | Scrolling length from top to hide automatically. `default: 420` |
| speed | Integer (ms) | The duration for scroll and fade speed. `default: 500` |
| position | boolean | You have this option whether you want to add custom position in css. Set this 'false' if you want to add custom position with your own css. `default: true` |
| right | Integer (px) | Position from right. (It will work only if 'position' is set 'true'.) `default: 15` |
| bottom | Integer (px) | Position from bottom. (It will work only if 'position' is set 'true'.) `default: 30` |

