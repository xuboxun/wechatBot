# wechatBot

## 说明
本项目用于我校信息学院每日晚上微信群汇报情况，考虑到辅导员工作辛苦、生保部同志统计工作量大，有同学提了一个Python的微信开发库，正好看到有Node.js版本的微信开发库，于是打算写一个机器人自动读取微信群消息，获取关键信息，自动导出Excel，省去大量的人工统计工作。  
本工具提供web界面，人机交互良好。  
沸点工作室web开发组提供技术支持。

## 安装&运行
``` bash
git clone git@github.com:xbx0119/wechatBot.git
cd wechatBot

# 后端
npm install

# 开发模式
npm run dev
# 生产模式
npm run release


# 前端
cd public
npm install

# 初始化
npm run init

# 开发模式
npm run dev
# 生产模式
npm run build

```


## 文件说明
1. bot/
    bot.js 读取微信消息，转发
2. lib/
    sendMsg.js 
    parseRegx.js 解析字符串
3. public/
    客户端代码


## 定义规则

robot://寝室号/是否到齐情况/未到人姓名及原因1/未到人姓名及原因2...

eg：
1. robot://荟五621/到齐
2. robot://荟五621/未到齐/黄一凡逸夫楼自习预计11点回
3. robot://荟五621/未到齐/黄一凡外出实习至某年某月/常见熊外出实习


## 控制台操作
1. 定义机器人运行时间
2. 定义