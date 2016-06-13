##接口文档
[TOC]
###同城
- 新增、更新同城  

	**url:** /adopt/addAdopt 
 
	**参数列表：**  
 	* content 必填，内容
 	* type 必填，类型   1 求助    2 雷锋  3 路过
 	* userId 必填，用户id
	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  

***  
- 查同城信息

	**url:** /adopt/queryAdopt 
 
	**参数列表：**  
	* userId 必填，信息发布人
 	* keyword 选填，标题
 	* longitude 必填
 	* latitude 必填
	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情    
***    
###脸谱
- 新增脸谱  

	**url:** /facebook/addFacebook 
 
	**参数列表：**  
 	* picList 必填，脸谱图片，字符串，多个时以,分割
 	* mainPic 必填，用户选择的主脸谱
 	* city 必填，城市
 	* userId 必填，用户id
	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  

***    
- 编辑脸谱

	**url:** /facebook/editFacebook 
 
	**参数列表：**  
	* userId 必填，信息发布人
 	* picList 选填，脸谱图片，字符串，多个时以,分割，与主图二选一
 	* mainPic 选填，主图
	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情    
***    
- 点赞脸谱  

	**url:** /facebook/upFacebook 
 
	**参数列表：**  
	* curUserId 必填，当前用户id
 	* userId 被点赞用户id，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情    
***    
- 踩脸谱  

	**url:** /facebook/downFacebook 
 
	**参数列表：**  
	* curUserId 必填，当前用户id
 	* userId 被踩用户id，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情    
***    
- 随机获取脸谱(16个)  

	**url:** /facebook/randomFacebook 
 
	**参数列表：**  
	* city 选填，城市，type为2时必填
 	* userId 选填，用户id，type为1时必填
 	* type 必填， 类型  1好友 2同城
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情    
***    
- 随机获取PK脸谱(4个)  

	**url:** /facebook/randomPkPhotos 
 
	**参数列表：**  
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情    
***    
- 查看脸谱  

	**url:** /facebook/findFacebook 
 
	**参数列表：**  
 	* userId 选填，用户id，type为1时必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情    
***    
###设备
- 新增设备  

	**url:** /device/addDevice 
 
	**参数列表：**  
	* userId 用户id，必填
 	* deviceName 设备名，必填
 	* deviceCode 设备编号，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情    
***    
- 查看设备列表 

	**url:** /device/findDeviceList 
 
	**参数列表：**  
	* userId 用户id，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息，success时为查询结果
 	* err 错误详情    
***    
- 删除设备 

	**url:** /device/deleteDevice 
 
	**参数列表：**  
	* userId 用户id，必填
	* deviceCode 设备编号，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情    
***    
###字典
- 新增字典 

	**url:** /dict/addDict 
 
	**参数列表：**  
	* key 必填
 	* value 选填 type为2时，以,分割  type为3时，为json字符串
 	* type 必填  1 值  2 list   3 object
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情    
***    
- 查字典 

	**url:** /dict/queryDict 
 
	**参数列表：**  
	* key 必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息，success时为查询结果
 	* err 错误详情    
***    
###设备配置
- 初始化设备配置信息 

	**url:** /globalDeviceConfig/initGlobalDeviceConfig 
 
	**参数列表：**  
	* userId 用户id，必填
 	* defaultDeviceId 设备id
 	* videoLength 视频时长，单位：秒，默认值100
 	* audioLength 音频时长，单位：秒，默认值100
 	* lightOnAlert 灯效开预警值，单位：分钟，默认值5
 	* lowChargeAlert 低电量预警值，例如25，代表25%，默认值25
 	* dataAutoSaveInterval 自动记录数据间隔，单位：分钟，默认值15
 	* dataAutoSendInterval 自动发送数据间隔，单位：分钟，默认值60
 	* autoCallInterval 自动呼叫间隔，单位：小时，0代表从不，默认值0
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情    
***    
- 查看设备配置信息 

	**url:** /globalDeviceConfig/findGlobalDeviceConfig 
 
	**参数列表：**  
	* userId 用户id，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息，success时为查询结果
 	* err 错误详情    
***    
- 更新设备配置信息 

	**url:** /globalDeviceConfig/updateGlobalDeviceConfig 
 
	**参数列表：**  
	* userId 用户id，必填
 	* defaultDeviceId 设备id
 	* videoLength 视频时长，单位：秒
 	* audioLength 音频时长，单位：秒
 	* lightOnAlert 灯效开预警值，单位：分钟，默认值5
 	* lowChargeAlert 低电量预警值，例如5，代表5%
 	* dataAutoSaveInterval 自动记录数据间隔，单位：秒
 	* dataAutoSendInterval 自动发送数据间隔，单位：分钟
 	* autoCallInterval 自动呼叫间隔，单位：小时，0代表从不
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情    
***    
- 重置设备配置信息 

	**url:** /globalDeviceConfig/resetGlobalDeviceConfig 
 
	**参数列表：**  
	* userId 用户id，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情    
***    
###健康
- 查看今天的步行数 

	**url:** /health/findDailyStepCount 
 
	**参数列表：**  
	* deviceId 设备id, 必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息，success时为查询结果
 	* err 错误详情  
***  
- 查看今天的饮食数 

	**url:** /health/findDailyEatCount 
 
	**参数列表：**  
	* deviceId 设备id, 必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息，success时为查询结果
 	* err 错误详情  
***  
- 查看今天的睡眠 

	**url:** /health/findDailySleepCount 
 
	**参数列表：**  
	* deviceId 设备id, 必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息，success时为查询结果
 	* err 错误详情  
***  
- 查看一周的健康数据 

	**url:** /health/findWeeklyHealthData 
 
	**参数列表：**  
	* deviceId 设备id, 必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
 	* weeklyStepCount 周运动步数
 	* weeklySleepCount 周睡眠数
***  
- 查看一月的健康数据 

	**url:** /health/findMonthlyHealthData 
 
	**参数列表：**  
	* deviceId 设备id, 必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
 	* monthlyStepCount 月运动步数
 	* monthlySleepCount 月睡眠数
***  
- 查看一年的健康数据 

	**url:** /health/findYearlyHealthData 
 
	**参数列表：**  
	* deviceId 设备id, 必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
 	* yearlyStepCount 年运动步数
 	* yearlySleepCount 年睡眠数
***  
- 查看健康榜单 

	**url:** /health/findTopList 
 
	**参数列表：**  
	* type 1 运动榜  2吃货榜  3懒鬼榜  4男神榜  5女生榜 不填时默认全榜
 	* period 按年、月、周查看，分别为0，1，2  必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息，success时为返回结果
 	* err 错误详情  
***  
###地图
- 查询附件的商家 

	**url:** /map/placeSearchService 
 
	**参数列表：**  
	* keywords 关键字，必填
 	* longitude 横坐标，必填
 	* latitude 纵坐标，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息，成功时返回商家列表
 	* err 错误详情  
***  
###商家
- 新增商家 

	**url:** /merchant/addMerchant 
 
	**参数列表：**  
	* userId 用户id，必填
 	* name 商家名称，必填
 	* phone 商家电话，必填
 	* storeName 店铺名称，必填
 	* area 省市区，必填
 	* storeAddress 店铺地址，必填
 	* mainPic 主图，必填
 	* storePicList 门店图片，必填，多个以,分隔
 	* storeCategory 店铺分类，必填
 	* longitude 横坐标，必填
 	* latitude 纵坐标，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息，成功时返回商家id
 	* err 错误详情  
 	***  
 	- 编辑商家 

	**url:** /merchant/editMerchant 
 
	**参数列表：**  
	* merchantId 商家id，必填
 	* userId 用户id，必填
 	* name 商家名称，选填
 	* phone 商家电话，选填
 	* storeName 店铺名称，选填
 	* area 省市区，选填
 	* storeAddress 店铺地址，选填
 	* mainPic 主图，选填
 	* status 审核状态，选填 0 新建  1 审核通过  2审核不通过
 	* businessTime 营业时间描述，选填
 	* storePicList 门店图片，选填，多个以,选填
 	* licensePicList 营业执照图片，选填，多个以,选填
 	* creditPicList 身份证图片，选填，多个以,选填
 	* productList 产品列表，选填 [{title : pic}, {title : pic}]
 	* storeCategory 店铺分类，选填
 	* longitude 横坐标，选填
 	* latitude 纵坐标，选填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
 	***  
- 查询附件的商家 

	**url:** /merchant/findNearestMerchant 
 
	**参数列表：**  
	* keyword 搜索关键字，必填
 	* longitude 当前位置，横坐标，必填
 	* latitude 当前位置，纵坐标，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息，success时为返回结果
 	* err 错误详情  
***  
- 查询商家 

	**url:** /merchant/findMerchant 
 
	**参数列表：**  
 	* userId 当前用户Id，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息，success时为返回结果
 	* err 错误详情  
***  
###文件、图片### 
- 上传文件--私有地址，需下载接口才能取到数据 

	**url:** /oss/upload 
 
	**参数列表：**  
	* filename 文件名，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
 	* url 返回的图片、文件链接  
***  
- 读文件，从私有地址读取文件字节流 

	**url:** /oss/download 
 
	**参数列表：**  
	* filename 文件名，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，error
 	* info 返回信息
 	* err 错误详情  
 	* 成功时为文件字节流，无msg，info，error字段  
***  
- 上传文件--公有地址，外网可访问 

	**url:** /oss/uploadPublic 
 
	**参数列表：**  
	* filename 文件名，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
 	* url 返回的图片、文件链接
***  
###宠物### 
- 新增宠物 

	**url:** /pet/addUserPet 
 
	**参数列表：**  
	* userId 用户id，必填
 	* nickName 宠物昵称，必填
 	* gender 性别，0 公  1 母，选填
 	* category 分类，必填
 	* categoryLeaf 子类别，必填
 	* deviceId 设备号，选填
 	* birthday 生日，选填
 	* weight 重量，选填
 	* picture 头像，选填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息，成功时为宠物id
 	* err 错误详情  
***  
- 查看宠物，3个参数可自由组合 

	**url:** /pet/findUserPets 
 
	**参数列表：**  
	* curUserId 当前用户id，必填
	* userId 用户id
 	* pId 宠物id
 	* deviceId 设备id
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息，成功时为查询结果
 	* err 错误详情  
***  
- 编辑宠物 

	**url:** /pet/updatePet 
 
	**参数列表：**  
	* userId 用户id，必填
 	* petId 宠物id，必填
 	* nickName 宠物昵称，选填
 	* deviceId 设备号，选填
 	* gender 性别 0 公  1 母，选填
 	* category 分类，选填
 	* categoryLeaf 子类别，选填
 	* birthday 生日，选填
 	* weight 重量，选填
 	* picture 头像，选填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
***  
- 删除宠物 

	**url:** /pet/deletePet 
 
	**参数列表：**  
	* userId 用户id，必填
 	* petId 宠物id，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
***  
- 点赞宠物 

	**url:** /pet/upPet 
 
	**参数列表：**  
	* userId 用户id，必填
 	* petId 宠物id，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
***  
- 查询宠物分类 

	**url:** /pet/queryPetCategoryList 
 
	**参数列表：**  
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息，成功时为查询结果
 	* err 错误详情  
***  
- 添加宠物分类 

	**url:** /pet/addPetCategory 
 
	**参数列表：**  
	* categoryName 大分类名  猫、狗
 	* categoryLeafName 二级分类
 	* petPic 宠物缩略图
 	* petPic 图片
 	* basicIntroduce 基本介绍
 	* categoryIntroduce 种类介绍
 	* origin 起源
 	* livingHabbit 生活习性
 	* feather 特征
 	* feedingWay 饲养方式
 	* advantage 优缺点
 	* distinct 相关区别
 	* eatingNotice 饮食须知
 	* washingTips 洗澡诀窍
 	* reproduceNotice 繁殖须知
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
***  
- 获取宠物百科 

	**url:** /pet/getPetWiki 
 
	**参数列表：**  
	* id 必填，宠物分类id
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
***  
###宠物日志
- 新增宠物日志 

	**url:** /petLog/addUserPetLog 
 
	**参数列表：**  
	* userId 用户id，必填
 	* petId 宠物id，必填
 	* content 内容，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
***  
- 查看宠物日志 

	**url:** /petLog/findUserPetLog 
 
	**参数列表：**  
	* petId 宠物id，必填
	* pageIndex 选填
 	* cookieId 必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息，成功时为查询结果
 	* err 错误详情  
***  
###帖子及评论
- 发布帖子，内容或图片至少二选一 

	**url:** /post/createPost 
 
	**参数列表：**  
	* title 帖子标题，必填
    * content 帖子内容，选填
	* picList 图片列表，选填，以,分割
	* userId 当前用户id，必填
	* longitude 当前位置横坐标，选填
	* latitude 当前位置纵坐标，选填
	* type 类型 1 空间    2喵吧    3空间&喵吧
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
***  
- 查看喵吧帖子 

	**url:** /post/findPost 
 
	**参数列表：**  
	* id 帖子id，选填
 	* userId 发帖人id，选填
 	* curUserId 当前用户id，必填
 	* pageIndex 非必填，默认1 当前页数
 	* pageSize 非必填，默认5 查询条数
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
 	* post 帖子详情，数组
***  
- 查看帖子评论，帖子id、评论id二选一，不能同时为空 

	**url:** /post/findPostComment 
 
	**参数列表：**  
	* id 帖子id
 	* commentId 评论id
 	* pageIndex 非必填，默认1 当前页数
 	* pageSize 非必填，默认5 查询条数
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息，成功时为评论详情，数组
 	* err 错误详情  
***  
- 查询帖子点赞信息 

	**url:** /post/findUpPostLog 
 
	**参数列表：**  
	* id 帖子id
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息，成功时为点赞详情，数组
 	* err 错误详情  
***  
- 编辑帖子 

	**url:** /post/editPost 
 
	**参数列表：**  
	* id 帖子id，必填
	* userId 当前用户id，必填
 	* title 帖子标题，选填
 	* content 帖子内容，选填
 	* picList 图片列表，选填，以,分割
 	* longitude 当前位置横坐标，选填
 	* latitude 当前位置纵坐标，选填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
***  
- 点赞帖子，一个用户不允许多次点赞，并通过极光接口发送消息给客户端，极光通过TAG标识，tagId为userId，需在APP端设置TAG 

	**url:** /post/upPost 
 
	**参数列表：**  
	* id 帖子id，必填
 	* userId 当前用户id，必填
 	* nickName 当前用户昵称，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
***  
- 点赞帖子评论，一个用户一天内不允许多次点赞，并通过极光接口发送消息给客户端，极光通过TAG标识，tagId为userId，需在APP端设置TAG 

	**url:** /post/upPostComment 
 
	**参数列表：**  
	* commentd 评论id，必填
 	* userId 当前用户id，必填
 	* nickName 当前用户昵称，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
***  
- 评论帖子，并通过极光接口发送消息给客户端，极光通过TAG标识，tagId为userId，需在APP端设置TAG 

	**url:** /post/addPostComment 
 
	**参数列表：**  
	* pid 帖子id，必填
 	* postUserId 发帖人用户id，必填
 	* comment 评论内容，选填，与图片列表至少一个
 	* picList 图片列表，选填，以,分割
 	* parentCommentId 父级评论id，选填
 	* userId 当前用户id，必填
 	* nickName 当前用户昵称，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
***  
- 逻辑删除帖子&评论 

	**url:** /post/deletePost 
 
	**参数列表：**  
	* userId 用户id，必填
 	* id 帖子id，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
***  
- 逻辑删除评论 

	**url:** /post/deletePostComment 
 
	**参数列表：**  
	* userId 用户id，必填
 	* pid 帖子id，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
***  
- 查看空间的帖子列表 

	**url:** /post/findFriendPostList 
 
	**参数列表：**  
	* userId 当前用户id
 	* pageSize
 	* pageIndex
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
***  
- 随机查看热帖 

	**url:** /post/findRandomHotPost 
 
	**参数列表：**  
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
***  
###建议
- 提交建议 

	**url:** /suggestion/saveSuggestion 
 
	**参数列表：**  
	* suggestion 意见，必填
 	* phone 电话，必填
 	* userId 用户id，选填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
***  
###用户位置
- 插入或更新用户当前位置（不存在时插入，存在时更新） 

	**url:** /userLocation/updateUserLocation 
 
	**参数列表：**  
	* userId，必填
 	* longitude，必填
 	* latitude，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
***  
- 查找附件最近的20个用户 

	**url:** /userLocation/findUserNearby 
 
	**参数列表：**  
	* userId 必填，当前用户id
	* longitude 必填
 	* latitude 必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息，success时有值，会包含当前用户自己，注意过滤，相差的距离，单位：米
 	* err 错误详情  
***  
###消息
- 查看消息列表 

	**url:** /message/findMessageList 
 
	**参数列表：**  
	* updateTime 上次更新时间
 	* userId 用户id
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
***  
- 增量获取系统消息列表 

	**url:** /message/getSysMessageList 
 
	**参数列表：**  
	* updateTime 上次更新时间
 	* target 发送对象，必填
 	* cookieId 登录时返回的cookieId，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 返回信息
 	* err 错误详情  
***  
###用户
- 发送手机验证码，注册，重置密码用 

	**url:** /user/sendPhoneVerifyCode 
 
	**参数列表：**  
 	* phone 电话，必填
 	* type 选填，1为注册  2为重置密码，不填时为2
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 
 	* err 错误详情  
 	* status 状态 0 电话为空 1 用户已注册 2 系统错误
***  
- 校验手机验证码 

	**url:** /user/validatePhoneVerifyCode 
 
	**参数列表：**  
 	* phone 必填
 	* verifyCode 必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 
 	* err 错误详情  
 	* status 状态 0 电话或验证码为空 1 验证码错误 2 系统错误  3验证码过期
***  
- 注册用户 

	**url:** /user/register 
 
	**参数列表：**  
 	* phone 手机号，必填
 	* password 密码，必填
 	* nickName 昵称，必填
 	* publicKey 公钥，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info
 	* err 错误详情  
 	* status 状态 0 电话或密码为空 1 系统错误  2 手机号已注册  3 验证码过期 4 缓存过期
***  
- 登录时校验用户名密码 

	**url:** /user/logIn 
 
	**参数列表：**  
 	* 手机号，必填
 	* password 密码，必填
 	* publicKey 公钥，必填
 	* uuid 客户端uuid，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info success时为公钥
 	* err 错误详情  
 	* cookieId 用于查询用户id
 	* userName 用于登录环信
 	* password 用于登录环信
 	* nickName 昵称
 	* status 0 必填参数为空  1 系统错误  2 用户名/密码错误  3 手机号未注册   4 缓存过期
***  
- 退出登录，此结果返回成功后需调环信接口退出环信 

	**url:** /user/logOut 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 客户端uuid
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info
 	* err 错误详情  
 	* status 1 系统错误
***  
- 重置密码 

	**url:** /user/resetPassword 
 
	**参数列表：**  
 	* phone 必填
 	* password 必填
 	* publicKey 公钥，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info
 	* err 错误详情  
 	* status 1 系统异常   2 手机号未注册  3 验证码过期 4 缓存过期 
***  
- 根据cookieId获取用户id信息 

	**url:** /user/getUser 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 成功时返回用户id
 	* err 错误详情  
***  
- 查询用户资料（3选1） 

	**url:** /user/findUserProfile 
 
	**参数列表：**  
 	* userId  用户id 字符串，选填，支持批量查询，以,分割，如"12124312455,233143543664"
 	* phone 用户手机 选填
 	* nickName 昵称 选填
 	* uuid 必填
 	* cookieId 必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 成功时返回用户资料
 	* err 错误详情  
***  
- 修改用户资料 

	**url:** /user/updateUserProfile 
 
	**参数列表：**  
 	* userId 用户id，必填
 	* cookieId 必填
 	* uuid 必填
 	* nickName 昵称，选填
 	* userPicture 头像，选填
 	* birthday 生日，选填，格式：YYYY-MM-DD, 如2016-01-26
 	* style 个性签名，选填
 	* barCode 二维码，选填
 	* status 状态，选填
 	* phone 电话，选填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 
 	* err 错误详情  
***  
- 新增消息免打扰好友、群 

	**url:** /user/addChatConfig 
 
	**参数列表：**  
 	* userId 当前用户id，即环信用户名，必填
 	* friendUserId 好友id，即好友环信名，选填
 	* groupId 群组id，选填
 	* cookieId 必填
 	* uuid 必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 
 	* err 错误详情  
***  
- 取消消息免打扰好友、群 

	**url:** user/cancelChatConfig 
 
	**参数列表：**  
 	* userId 当前用户id，即环信用户名，必填
 	* friendUserId 好友id，即好友环信名，选填
 	* groupId 群组id，选填
 	* cookieId 必填
 	* uuid 必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 
 	* err 错误详情  
***  
- 查看消息免打扰好友、群 

	**url:** /user/findChatConfig 
 
	**参数列表：**  
 	* userId 当前用户id，即环信用户名，必填
 	* friendUserId 好友id，即好友环信名，选填
 	* groupId 群组id，选填
 	* cookieId 必填
 	* uuid 必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 
 	* err 错误详情  
 	* status 成功时有值  1 已设置免打扰  0 未设置免打扰
***  
- 举报好友/群，如果有图片，多个图片url通过,分割；被举报好友、群组必须二选一 

	**url:** /user/report 
 
	**参数列表：**  
 	* userId 当前用户id，即环信用户名，必填
 	* friendUserId 好友id，即好友环信名，选填
 	* groupId 群组id，选填
 	* content 内容，必填
 	* picUrlList 图片列表，非必填
 	* cookieId 必填
 	* uuid 必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info
 	* err 错误详情  
***  
- 发起遛弯邀请，并通过极光接口推送 

	**url:** /user/sendWalkRequest 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 必填
 	* userId 当前用户id，必填
 	* nickName 当前用户昵称，必填
 	* gusetUser 遛弯邀请的对象，值为用户id的数组
 	* longitude 选填
 	* latitude 选填
 	* address 选填
 	* meetLongitude 选填
 	* meetLatitude 选填
 	* meetAddress 选填
 	* petName 选填，宠物名
 	* petCategory 选填，宠物分类
 	* meetTime 选填，不填时为当前时间 格式YYYY-MM-DD HH:MI:SS
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info
 	* err 错误详情  
***  
- 添加好友 

	**url:** /user/addFriend 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 必填
 	* userId 当前用户id，必填
 	* friendId 好友id，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 
 	* err 错误详情  
***  
- 删除好友 

	**url:** /user/deleteFriend 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 必填
 	* userId 当前用户id，必填
 	* friendId 好友id，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 
 	* err 错误详情  
***  
- 获取好友列表 

	**url:** /user/getFriendList 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 必填
 	* userId 当前用户id，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info success时好友列表
 	* err 错误详情  
***  
- 添加黑名单 

	**url:** /user/addBlackFriend 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 必填
 	* userId 当前用户id，必填
 	* friendId 好友id，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 
 	* err 错误详情  
***  
- 删除黑名单好友 

	**url:** /user/deleteBlackFriend 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 必填
 	* userId 当前用户id，必填
 	* friendId 好友id，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 
 	* err 错误详情  
***  
- 获取黑名单好友列表 

	**url:** /user/getBlackFriendList 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 必填
 	* userId 当前用户id，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info success时为黑名单列表
 	* err 错误详情  
***  
- 查看用户是否在黑名单列表 

	**url:** /user/checkUserInBlackFriendList 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 必填
 	* userId 当前用户id，必填
 	* friendId 好友id，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info success且值为1时，表示在黑名单列表，为0表示不在黑名单列表
 	* err 错误详情  
***  
- 获取加入的群列表 

	**url:** /user/getGroupList 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 必填
 	* userId 当前用户id，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info success时为加入的群列表
 	* err 错误详情  
***  
- 获取群信息（包括群名、成员列表、创建时间） 

	**url:** /user/getGroupMemberList 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 必填
 	* groupId 群组id，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info success时为群信息
 	* err 错误详情  
***  
- 根据群名查找群 

	**url:** /user/findGroup 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 必填
 	* groupName 群组名，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info success时为群列表
 	* err 错误详情  
***  
- 创建群 

	**url:** /user/createGroup 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 必填
 	* groupName 群组名，必填
 	* userId 当前用户id，必填
 	* memberList 群成员列表，必填，多个时以,分隔
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 成功时为群id
 	* err 错误详情  
***  
- 管理群（支持自己主动加群退群） 

	**url:** /user/editGroup 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 必填
 	* userId 当前用户id，必填
 	* id 群id，必填
 	* memberAdd 添加的群成员，选填
 	* memberDel 删除的群成员，选填
 	* status 群状态， 1表示解散，选填
 	* groupName 群组名，选填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 
 	* err 错误详情  
***  
- 保存好友请求 

	**url:** /user/saveFriendRequest 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 必填
 	* userId 当前用户id，必填
 	* nickName 当前用户昵称，必填
 	* guestUser 被请求添加的好友id，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 成功时为请求id
 	* err 错误详情  
***  
- 保存群添加申请 

	**url:** /user/saveGroupRequest 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 必填
 	* userId 当前用户id，必填
 	* nickName 当前用户昵称，必填
 	* guestUser 被请求添加的好友id，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 
 	* err 错误详情  
***  
- 查看好友请求列表 

	**url:** /user/findFriendRequest 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 必填
 	* userId 当前用户id，必填
 	* type 请求类型  1 发起的  2 收到的， 不填时两个都查，非必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info success时为好友请求列表
 	* err 错误详情  
***  
- 更新好友请求状态 

	**url:** /user/updateFriendRequestStatus 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 必填
 	* userId 当前用户id，必填
 	* requestId 请求id，必填
 	* status 状态 1同意  2拒绝，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info 
 	* err 错误详情  
***  
- 查看加群申请 

	**url:** /user/findGroupRequest 
 
	**参数列表：**  
 	* cookieId 必填
 	* uuid 必填
 	* userId 当前用户id，必填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info success时为群请求列表
 	* err 错误详情  
***  
- 获取公钥，用于对敏感信息加密，有效期3分钟，无需入参 

	**url:** /user/generatePublicKey 
 
	**参数列表：**  
 	* 无
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* info success时为公钥
 	* err 错误详情  
 	* status 1 系统错误  
***  
- 第三方登录（第一次登录会创建一个新用户）

	**url:** /user/thirdPartLogin 
 
	**参数列表：**  
 	* openId 必填
 	* openType 必填
 	* uuid，必填
 	* nickName，选填
 
	**返回值列表：**
 	* msg 返回码，success/error
 	* cookieId 
	* userName 
	* password
	* nickName
 	* err 错误详情  
 	* status 0 必填参数为空  1 系统错误 2 帐号异常  
***  