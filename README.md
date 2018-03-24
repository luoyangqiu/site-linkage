# site-linkage 主要提供JSON格式的省市区三级联动数据
创建初衷：
由于项目所需，需要一份较新的中国各地省市县区的三级联动数据！不过经过几天的时间在网上搜集，发现确实没有较新的数据，或多或少有些缺陷，另外也发现不少人有这样的需求，因此自己花时间搜集了一份省市县区的三级联动数据，后期还会持续更新！有需要的朋友可以持续关注
本插件只提供数据源和基末的数据查询方式！
# 数据来源
数据采集整理来自各地方政府的网上政务中心行政区域信息

# 使用方式

``` bash
npm install site-linkage
```

``` javascript
const siteLinkage = require('site-linkage')
//siteLinkage.data  获取所有省的数组
//["北京市", "天津市", "河北省", "山西省", "内蒙古", "辽宁省", "吉林省", "黑龙江省", "上海市", "江苏省", "浙江省", "安徽省", "福建省", "江西省", "山东省", "河南省", "湖北省", "湖南省", "广东省", "广西", "海南省", "重庆市", "四川省", "贵州省", "云南省", "西藏", "陕西省", "甘肃省", "青海省", "宁夏", "新疆", "台湾省", "澳门", "香港"]

//siteLinkage.getProvince('四川省').data  获取四川省下面所有的市的数组
["成都市", "自贡市", "攀枝花市", "泸州市", "德阳市", "绵阳市", "广元市", "遂宁市", "内江市", "乐山市", "南充", "眉山市", "宜宾市", "广安市", "达州市", "雅安市", "巴中市", "资阳市", "阿坝藏族羌族自治州", "甘孜藏族自治州", "凉山彝族自治州", "其他"]

//siteLinkage.getProvince('四川省').getCity('成都市').data  获取四川省成都市下面所有的区县的数组
["高新区", "天府新区", "青羊区", "锦江区", "金牛区", "武侯区", "成华区", "龙泉驿区", "青白江区", "新都区", "温江区", "都江堰市", "彭州市", "邛崃市", "崇州市", "金堂县", "郫都区", "新津县", "双流县", "蒲江县", "大邑县", "简阳市", "其他"]

```

# 采集方式和问题反馈
目前主要是手动采集，后期会抽时间，添加爬虫自动采集，并且希望各位网友发现数据问题之后可以与我联系：505072907@qq.com  


