# cdn
## hexo jsdelive cdn
建立CDN库，通过 jsdelivr 引用资源
- 使用方法：https://cdn.jsdelivr.net/gh/ 你的用户名 / 你的仓库名 @发布的版本号 / 文件路径
-举例：
1. https://cdn.jsdelivr.net/gh/zyhcs/cdn@1.0/medias/avatars/avatar.jpg
2. https://cdn.jsdelivr.net/gh/zyhcs/cdn@1.0/medias/music/song/倒数.mp3
3. https://cdn.jsdelivr.net/gh/zyhcs/cdn@1.0/source/_data/music.json

> == 注意：== 版本号不是必需的，是为了区分新旧资源，如果不使用版本号，将会直接引用最新资源

- 后期资源更新：如果以后在向 cdn 库里添加或者修改文件，首先把文件添加到本地仓库，然后依次在本地 cdn 仓库文件位置执行以下命令：
```git
git pull origin master  #拉取远程仓库到本地
git add .
git commit -m '描述内容'
git push origin master  # 推送到GitHub仓库
```
——然后在执行版本发布的操作，引用链接即可。
最后感谢大佬[过客～励む](https://yafine-blog.cn/)的建库教程，本库的搭建参考大佬的文章[使用 Jsdelivr/CDN 加速博客访问速度](https://yafine-blog.cn/posts/ee35.html)。
