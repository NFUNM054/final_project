# API_期末项目

### [20×20产品介绍](https://gitee.com/NFUNM054/API_final_project/blob/master/%E7%9B%8A%E8%B5%B7%E6%9D%A5APP_%E4%BA%A7%E5%93%81%E4%BB%8B%E7%BB%8D.pptx)

| 史诗      | “益起来”APP |
| ------------ | ------------- |
| 发布日期     | 2019年12月    |
| 文件状态     | 进行中        |
| 文件主人     | 林梓仪        |
| 领头的设计师 | 林梓仪        |
| 领头的开发者 | 林梓仪        |
| 领头的测试者 | 林梓仪        |


-------
## 目标
让有减肥以及塑身需求却不知道自己每天所摄入食物的卡路里量的人群，可以通过这个APP了解自身的身体指数，以及每天摄入的卡路里量，让他们能够更加有效率的减肥和塑身。

## 目标人群
减肥塑身人群

## 背景
- 2019年2月，世界卫生组织调查报告显示，当今65亿人口中，有16亿人超重。中国肥胖人群约2亿，排名第148位，但因随着中国的经济增长，人们的生活水平不断提高，肥胖人群也在增加，且速度惊人。中国的肥胖人数比1992年以来增长了近3倍。

- 肥胖和超重的根本原因是摄入卡路里与消耗卡路里之间的能量不平衡。目前造成超重与肥胖的主要原因有三点：运动过少，营养过剩，遗传因素。

- 超重和肥胖是罹患非传染性疾病的重大风险因素，比如：心血管疾病（特别是心脏病和中风），糖尿病，骨关节炎等。

- 目前很多人在减肥方式上存在着很多问题，例如节食减肥、药物减肥甚至吸脂减肥等不健康的减肥方式，这些减肥方式很容易对身体造成严重的后果。所以倡导健康减肥是非常有必要的。

- 随着经济水平的发展，人们已经解决了温饱问题，更加注重外观上的问题。因此，想要减肥塑身的人越来越多，但因为许多人不了解自身的身体指数以及哪些食物中的热量的多少，导致有些人一直减肥塑身不成功。

## 一、价值主张设计
### 加值宣言 
#### 一句话版本
该APP分别使用了标准体重计算器API、百度AI的菜品识别API和果蔬识别API以及营养成分表API，为用户检测BMI指数，让用户了解自己所摄入食物的热量，并向用户推荐合理的运动量。

#### 一分钟版本
该APP使用了极速数据里的标准体重计算器API，将会给用户评估她的BMI指数，让她能够更加了解自身身体水平，能够对减肥塑身进行更完善的规划。使用了百度AI的菜品识别API，用户通过拍照/上传可以识别出菜品的热量以及置信度。让用户可以更好的了解到他所食用的菜品的热量。为了清楚得知用户食用的份量，该APP设置了选择“选择份量”以及“选择数量”来更好的预测卡路里。在系统分析完菜品后，将为用户呈现菜品识别结果、卡路里含量和脂肪转化量等信息，并向用户推荐合理的运动量。
该APP也运用百度AI的果蔬识别API和天行数据里的营养成分表API，用户可以通过拍照/上传图片识别果蔬，然后查看果蔬里的营养成分来了解这个果蔬是否适合在减肥/塑身的时候食用。

### 核心价值（最小可行性产品）
- 该APP的核心价值是用户可以通过拍照/上传菜品的图片识别出食物的热量，以此来了解自己所摄入食物的热量，并向用户推荐合理的运动量。


### 核心价值与用户痛点
- 传统的健康管理类软件需要手动输入每天的卡路里摄入量，操作繁杂且热量统计不准确，并无法根据摄入热量推荐合理的运动量，导致用户的运动消耗和饮食摄入的热量不均衡，不利于用户知道其每天的运动量，摄入量，为之后的健康减肥做准备。

- 用户无法清楚知道每天自己摄入多少热量。

- 用户无法通过得知自己摄入多少热量，来规划每日运动量。


### 人工智能概率性与用户痛点
- 百度AI中的菜品识别API准确度高达85%，虽然准确度较高，但如果用户的图片中有两个菜品，是无法准确识别的，且相似菜品容易判断出错。

### 需求列表与人工智能API加值
| 需求                     | 重要程度 | API               |
| ------------------------ | -------- | ----------------- |
| 用户想要知道每日摄入的热量     | ♥♥♥♥♥   | 图像识别-菜品识别 |
| 用户想要知道自身的BMI指数 | ♥♥♥♥   | 标准体重计算器API   |
| 用户想要知道果蔬里的营养成分  | ♥♥♥ | 营养成分表API   |
| 用户想要知道这个是什么果蔬  | ♥♥ | 图像识别-果蔬识别  |


## 二、原型
### 交互式及界面设计
#### BMI指数
![BMI指数_交互.JPG](https://upload-images.jianshu.io/upload_images/9476218-3c398eadfc162cd9.JPG?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
- 上图为在登录APP后，用户需先对自己的BMI指数进行测试，用户输入自己的性别、体重和身高，就会帮助用户计算出BMI指数。让用户可以判断自己的BMI指数是否低于或高于正常值（高于正常值则偏胖，低于正常值则偏瘦），以此对运动和饮食进行调整，以便减肥/塑身。该功能使用了极速数据里的标准体重计算器API。

#### 菜品识别
![菜品识别_交互.JPG](https://upload-images.jianshu.io/upload_images/9476218-c2f79e87cb43cf14.JPG?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
- 上图为用户通过拍照/上传可以识别出菜品的热量以及置信度。让用户可以更好的了解到他所食用的菜品的热量。该功能使用了百度AI图像识别中的菜品识别。

#### 果蔬识别和营养成分表API 
![果蔬识别_交互.JPG](https://upload-images.jianshu.io/upload_images/9476218-78869e4ce8ada57c.JPG?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
- 用户可以通过拍照/上传识别果蔬，然后查看果蔬里的营养成分来了解这个果蔬是否适合在减肥/塑身的时候食用。该功能使用了百度AI的果蔬识别API以及天行数据里的营养成分表API。

### 信息设计

#### 产品架构图
![产品架构图.JPG](https://upload-images.jianshu.io/upload_images/9476218-3432d276e0da81c1.JPG?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

#### 产品核心功能架构图
![产品核心功能架构图.JPG](https://upload-images.jianshu.io/upload_images/9476218-6d1bed9ad17334d7.JPG?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

#### 产品流程图
![益起来APP流程图.jpg](https://upload-images.jianshu.io/upload_images/9476218-cbb56f1cf6eeedb3.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

### 原型文档
- [查看“益起来”原型](http://nfunm054.gitee.io/api_final_project/)
- [下载“益起来”原型rp文档](https://gitee.com/NFUNM054/API_final_project/blob/master/API%E2%80%94%E2%80%94%E7%9B%8A%E8%B5%B7%E6%9D%A5%E5%8E%9F%E5%9E%8B.rp)

### 口头操作说明

## 三、API 产品使用关键AI或机器学习之API的输出入展示 
### API使用水平
#### 标准体重计算器API
[查看标准体重计算器API之输入及输出](https://github.com/NFUNM054/final_project/blob/master/API%E6%B5%8B%E8%AF%95%E6%B0%B4%E5%B9%B3_%E6%A0%87%E5%87%86%E4%BD%93%E9%87%8D%E8%AE%A1%E7%AE%97%E5%99%A8API.md)

#### 菜品识别API
[查看菜品识别API之输入及输出](https://github.com/NFUNM054/final_project/blob/master/API%E6%B5%8B%E8%AF%95%E6%B0%B4%E5%B9%B3_%E8%8F%9C%E5%93%81%E8%AF%86%E5%88%ABAPI.md)

#### 果蔬识别API
[查看果蔬识别API之输入及输出](https://github.com/NFUNM054/final_project/blob/master/API%E6%B5%8B%E8%AF%95%E6%B0%B4%E5%B9%B3_%E6%9E%9C%E8%94%AC%E8%AF%86%E5%88%ABAPI.md)

#### 营养成分表API
[查看营养成分表API之输入及输出](https://github.com/NFUNM054/final_project/blob/master/API%E6%B5%8B%E8%AF%95%E6%B0%B4%E5%B9%B3_%E8%90%A5%E5%85%BB%E6%88%90%E5%88%86%E8%A1%A8API.md)

### 使用比较分析
#### 营养成分表API
- 经过的查找，我仅在天行数据中找到营养成分表API，因此无法进行使用比较分析。但经过我的使用，我发现了此API的示例代码是python2.7版本写的，未能与时俱进。且营养成分的返回结果有时不准确。因此，如若我找到了相较于天行数据的营养成分表API好的接口，将会进行替换。
- [天行数据营养成分表API接口](https://www.tianapi.com/apiview/121)

#### 标准体重计算器API
- 以下为极速数据和APIShop的标准体重计算器API对比与检测，我目前仅找到这两家有标准体重计算器API接口。

|   平台  |  功能   |  功能描述    |  返回结果   |  成熟度   |  性价比   |文档链接|
| --- | --- | --- | --- | --- | --- | --- |
|   极速数据  |标准体重计算器 |标准体重计算器、对照表，通过身高和体重来计算您的身材是否标准。国际比较权威的BMI指数计算。|bmi（BMI指数）、normbmi（正常BMI指数）、idealweight（理想体重）、level（水平）、danger（相关疾病发病的危险）、status（是否正常）|  ⭐⭐⭐⭐   |  高   |[极速数据文档](https://www.jisuapi.com/api/weight/)|
| APIShop    |标准体重计算器 | 身体质量指数 (Body Mass Index, 简称BMI), 通过身高和体重来计算您的身材是否标准。| 标准体重、标准身高| ⭐⭐    |  低   |[APIShop文档](https://www.apishop.net/#/api/detail/?productID=104)|

经过我的对比发现，极速数据的标准体重计算器API返回的数据相对较多，符合我这个APP所需要的要求。且示例代码相对符合我们所学的代码，因此我选择了极速数据下的体重计算器API。

#### 菜品识别API
- 以下为百度AI和聚合数据的菜品识别API对比，经过我的查找，发现这两家较符合我APP的需求，因此对其进行对比。

|   平台  |  功能   |  功能描述   |  返回结果   |  成熟度   |  性价比   |文档链接|
| --- | --- | --- | --- | --- | --- | --- |
|   百度AI  |菜品识别API |别超过9千种菜品，适用于识别只含有单个菜品的图片，接口返回菜品的名称、置信度、卡路里、百科信息等综合信息|菜品名称、卡路里，每100g的卡路里含量、识别结果中每一行的置信度值、对应识别结果的百科词条名称、对应识别结果百度百科页面链接、对应识别结果百科图片链接、对应识别结果百科内容描述。|  ⭐⭐⭐⭐   |  高   |[百度AI文档](https://ai.baidu.com/tech/imagerecognition/dish)|
| 聚合数据    |菜品识别API | 根据上传的菜品图片，识别菜品信息，如：菜品名称、卡路里信息、置信度。| 菜品名称、卡路里，每100g的卡路里含量、百科词条名称，可能为空、百科图片链接，可能为空、百科内容描述，可能为空| ⭐⭐⭐   |  中   |[聚合数据文档](https://www.juhe.cn/docs/api/id/372)|

经过我的对比发现，百度AI比较符合我的要求。百度AI菜品识别API成熟度高于聚合数据，百度AI拥有示例代码，而聚合数据没有。且百度AI拥有自身的图库，因此我选择了百度AI。

### 果蔬识别API
- - 以下为百度AI和聚合数据的果蔬识别API对比，经过我的查找，发现这两家较符合我APP的需求，因此对其进行对比。

|   平台  |  功能   |  功能描述   |  返回结果   |  成熟度   |  性价比   |文档链接|
| --- | --- | --- | --- | --- | --- | --- |
|   百度AI  |果蔬识别API |识别近千种水果和蔬菜的名称，适用于识别只含有一种果蔬的图片，可自定义返回识别结果数，适用于果蔬介绍相关的美食类APP中。|果蔬名称、置信度|  ⭐⭐⭐⭐   |  高   |[百度AI文档](https://ai.baidu.com/tech/imagerecognition/ingredient)|
| 聚合数据    |果蔬识别API | 精确识别近千种水果和蔬菜的名称，适用于识别只含有一种果蔬的图片，适用于果蔬介绍相关的美食类APP中。| 果蔬名称、置信度| ⭐⭐⭐   |  中   |[聚合数据文档](https://www.juhe.cn/docs/api/id/393)|

经过我的对比发现，百度AI比较符合我的要求。百度AI果蔬识别API成熟度高于聚合数据，百度AI拥有示例代码，而聚合数据没有。且百度AI拥有自身的图库，因此我选择了百度AI。

### 使用后风险报告
#### 百度AI之果蔬识别API和菜品识别API
##### API市场竞争程度
市场上的果蔬识别API和菜品识别API开放的平台比较多，因此百度AI的竞争对手是较多的。但百度AI的竞争优势在于他拥有自己的图库，且支持自定义菜品识别。菜品识别的准确度超过85%，在同类型的产品是相对较高的。因此在API市场竞争中优势较大。

##### API输出输入限制
请求限制：使用示例代码前，请记得替换其中的示例Token、图片地址或Base64信息。
图片格式：jpg/png/bmp格式
请求参数限制：图像数据，base64编码，要求base64编码后大小不超过4M，最短边至少15px，最长边最大4096px,支持jpg/png/bmp格式。注意：图片需要base64编码、去掉编码头（data:image/jpg;base64,）后，再进行urlencode。
返回参数分析：百度AI的果蔬识别API和菜品识别API仅能识别只含有一种果蔬/菜品的图片。

##### 定价
图像识别下各个能力都具有免费调用额度，开通付费后，每日免费调用额度仍保留，固定次数免费额度用完后需付费使用，免费额度：菜品识别API免费调用额度为500次/日，果蔬识别为共3000次（不限天数）

- 百度AI价格对比

![百度AI价格对比.JPG](https://upload-images.jianshu.io/upload_images/9476218-1e06e9566cdd7b70.JPG?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

- 菜品识别价目表

![菜品识别价目表.JPG](https://upload-images.jianshu.io/upload_images/9476218-1fb78660dbd1565e.JPG?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

- 果蔬识别价目表

![果蔬识别价目表.JPG](https://upload-images.jianshu.io/upload_images/9476218-4df89dc47e31ddbb.JPG?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

##### 相关链接
- [百度AI市场](https://aim.baidu.com/product/f7ee8543-ea10-457c-9183-1b9f2eddfcc3)
- [百度AI图像识别文档](https://ai.baidu.com/ai-doc/IMAGERECOGNITION/Kk3bcxbxj)
- [百度AI定价文档](https://ai.baidu.com/ai-doc/IMAGERECOGNITION/rk3bcxa9e)

### 加分项
使用了2个以上机器学习与人工智能API之输入输出

### 所使用的API文档
- [天行数据营养成分表API接口](https://www.tianapi.com/apiview/121)
- [百度AI菜品识别API接口](https://ai.baidu.com/tech/imagerecognition/dish)
- [百度AI果蔬识别API接口](https://ai.baidu.com/tech/imagerecognition/ingredient)
- [极速数据标准体重计算器API接口](https://www.jisuapi.com/api/weight/)
