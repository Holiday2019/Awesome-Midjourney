本文主要讲的是如何编写Prompts提示词中的描述信息。

# Midjourney图片生成基本原则

1. Midjourney具有语义联想功能，比如你让它画一个客厅，那就不必告诉它画沙发、电视机等这些客厅应有的元素(如果你不想要电视机，你可以用`-no television`)。
2. 描述信息中，越前面的词，权重越大，AI会参考的越多
3. 描述信息不需要写太多，后面的词权重太小，AI不太会考虑。后面的词，即便你描述了，可能AI也不一定给你画出来（不如先生成一张，然后慢慢投喂）。
4. 对于做一幅特别好的图来说，需要的专业知识很多（比如说光线），普通人很难把这些描述地又专业又面面俱到。

综上，<strong style="color:blue;">不要写太长的小作文，写关键词即可</strong>。

# Midjourney图片生成描述信息公式

| 序号 | 描述内容  | 举例说明                                       |
| ---- | --------- | ---------------------------------------------- |
| 1    | 形式      | 照片、插画……                                   |
| 2    | 主题内容  | 一只可爱的猫、山脉、一对父子正在聊天……         |
| 3    | 环境/背景 | 明亮的、昏暗的……                               |
| 4    | 灯光      | 自然光线、电影光……                             |
| 5    | 颜色      | 红色、蓝色……                                   |
| 6    | 构图      | 水平构图、对角线构图；俯视、正视……             |
| 7    | 镜头      | 焦距、光圈、曝光时间、ISO、                    |
| 8    | 参考方向  | 齐白石、张大千；导演王家卫；模仿香奈儿的风格…… |
| 9    | 渲染方式  | OC渲染、C4D渲染……（适合做3D形状）              |
| 10   | 图像设定  | 质量8K、尺寸16:9……                             |

事实上，这几个描述内容，写起来并不容易，有些非常专业。

那么，第一，我们该怎么读懂这些描述信息呢？这可以利用现成的工具。

1. [OPS/OpenPromptStudio | 可视化编辑提示词](https://github.com/Moonvy/OpenPromptStudio)

   

第二，我们该怎么写呢？——利用已有的描述信息来编写自己的描述信息。具体来说，又有以下3种方法。

1. 直接套用或模仿现有照片的拍摄参数，让生成的图片像图库里那样有质感。
2. 拆解网络上优秀Midjourney作品的关键词。
3. 使用Midjourney的describe功能。

# 方法1：使用照片的拍摄参数

## 方法介绍

网上看见一个摄影作品很好，想要生成类似风格的照片，怎么做？

- 假定你是在[Unsplash](https://unsplash.com/photos/a-woman-walking-down-a-sidewalk-next-to-a-tall-building-tyoyJFQUp1c)上找到的图片，可以看看该图有没有附带拍摄参数，如果有，将会是这样![image-20230703232329091](https://picture-cloud-master.oss-cn-hangzhou.aliyuncs.com/img202307032323215.png)

- 复制该拍摄参数

- 描述信息可以这么写
  ```
  Camera,SONY,ILCE-7M3,Lens,85.00mm f/1.4,1/60s,ISO 160 --ar 1:1 --v 5 --s 5

## 一个例子

没有摄影参数：

对比度没那么强，图片质感比较差

![image-20230703232949792](https://picture-cloud-master.oss-cn-hangzhou.aliyuncs.com/img202307032329863.png)

有摄影参数：

人像聚焦，质感较强

![示例1](https://picture-cloud-master.oss-cn-hangzhou.aliyuncs.com/img202307032330061.png)

![示例2](https://picture-cloud-master.oss-cn-hangzhou.aliyuncs.com/img202307032331531.png)

# 方法2：拆解网络上优秀作品的关键词

网络上专门有网站卖提示词的，也有一些是免费的。就像网友们分享ChatGPT提示词一样

1. [PromptHero中文官网：AI绘画Prompt提示词、关键描述词、参数指令大全](https://promptheroes.cn/)
2. 小红书相关博主
   - [AIGC鹿视界](https://www.xiaohongshu.com/user/profile/5944e7e750c4b47433f05620)
   - [AI学习笔记](https://www.xiaohongshu.com/user/profile/6073d38d00000000010068a6?xhsshare=CopyLink&appuid=6073d38d00000000010068a6&apptime=1679646639)
   - [鹿与熙🐰 ](https://www.xiaohongshu.com/user/profile/54e89d93d39ea2225c500f52)

# 方法3：利用Midjourney的describe功能

具体请见[05_学会垫图思维，快速生成意向图片](.\05_学会垫图思维，快速生成意向图片.md)