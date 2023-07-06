输入`/settings`，弹出以下内容。

![image-20230703205032184](https://picture-cloud-master.oss-cn-hangzhou.aliyuncs.com/img202307032103253.png)

设置，主要包括三块内容：模型、风格化、模式

# 模型

MJ：适合生成实景类图片

Niji：适合生成二次元插画类图片

```
用`--niji 5`、`--MJ 5`这样的代码来表示该参数
```

![image-20230703202301899](https://picture-cloud-master.oss-cn-hangzhou.aliyuncs.com/img202307032103388.png)

# 风格化

可以理解为“一个人思考的程度”

Stylize low：不思考，提示词是什么，就怎么画

Stylize med：AI稍加思考

Stylize high：有较多AI自己的思考

Stylize very high：有非常多AI自己的思考

（类似于ChatGPT的思维发散程度，就看你想要它准确严谨还是灵活创新了）

默认参数：--s 50

```
用`--s 50`、`--s 750`这样的代码来表示该参数
```

下面2组图中，明显右边的AI更有自己的想法，四幅图差异也比较大

![image-20230703202838155](https://picture-cloud-master.oss-cn-hangzhou.aliyuncs.com/img202307032103409.png)

## 一个经验——关于S值高低的设置

绘制<strong style="color:blue;">图标</strong>，尽量调低S值
绘制<strong style="color:blue;">图片</strong>，尽量<strong style="color:red;">调高</strong>S值

对于图标来说，内容较少，我们想要的就是我们描述的

![image-20230703203234535](https://picture-cloud-master.oss-cn-hangzhou.aliyuncs.com/img202307032103456.png)

# 模式

Public mode：在公共模式和私人模式之间切换。公共模式，你画的图会放在大厅里，别人也能看见你的提示词和绘图结果；私人模式则只有你自己可以看到。对应于`/public`和`/stealth`命令。
Remix mode：切换到混合模式，用于对图片某个局部位置微调。
High Variation Mode：让一组图像中的 4 张图像，差异更加明显。
Low Variation Mode：让一组图像中的 4 张图像，差异程度较小。
Turbo mode：使出图速度大幅提升。
Fast mode：快速出图。
Relax mode：在Fast 和 Relaxed 模式之间切换。对应于`/fast`和`/relax`命令。
Reset Settings：重置设置。

