# Vless for Daki.cc

* * *

# 目录

- [项目特点](README.md#项目特点)
- [部署](README.md#部署)
- [鸣谢下列作者的文章和项目](README.md#鸣谢下列作者的文章和项目)
- [免责声明](README.md#免责声明)

* * *

## 项目特点:
* 本项目用于在 [Daki.cc](https://daki.cc/) 免费服务上部署 VLESS
* 集成哪吒探针，可以自由选择是否安装
* 因为给到的端口不在 Cloudflare 的免费服务回源端口列表里，所以不能用 cdn 或者 workers
* Cloudflare HTTP流量可以使用的回源端口如下：80、8080、8880、2052、2082、2086、2095
* Cloudflare HTTPS流量可以使用的回源端口如下：443、2053、2083、2087、2096、8443

## 部署:
* 注册 [Daki.cc](https://daki.cc/)
* config.json 的 17 行修改 UUID
* server.js 的 4 行修改自己的 端口， 44 行修改哪吒参数
* 部署成功后 velss ws 的路径为: `/api`，如要修改，可以寻找并替换 server.js 的 90、96、97 行里的 api
* 需要应用的 js
  | 命令 | 是否必须 | 说明 |
  | ------------ | ------ | ------ |
  | <URL>/start | 是 | 运行 vless |
  | <URL>/nezha | 否 | 运行哪吒 |
  | <URL>/api | 否 | 查看 vless 运行结果 Bad Request 即是 OK |
  | <URL>/status | 否 | 查看后台进程  |

<img width="1658" alt="image" src="https://user-images.githubusercontent.com/62703343/212581034-4f0d9855-f223-43a1-aebe-f03b53aa56c3.png">
  
  
<img width="1107" alt="image" src="https://user-images.githubusercontent.com/62703343/212581110-565f57af-17e8-4ff3-85d7-d59d807ae2a5.png">
  
  
<img width="1171" alt="image" src="https://user-images.githubusercontent.com/62703343/212581198-58a28b24-3f9a-49fd-81bd-2f298a64478a.png">
  
  
<img width="1048" alt="image" src="https://user-images.githubusercontent.com/62703343/212581243-fbcfbe97-b39e-4524-9aff-c963cadbdc30.png">
  
  
<img width="1674" alt="image" src="https://user-images.githubusercontent.com/62703343/212581474-f50a5c8a-7e4f-49e3-85bd-be37b28e0686.png">
  
  
<img width="1672" alt="image" src="https://user-images.githubusercontent.com/62703343/212581572-854b0ca6-49b1-4882-b6c4-c1a3f817aa63.png">
  
  
<img width="1198" alt="image" src="https://user-images.githubusercontent.com/62703343/212582001-414cf1b6-6cf2-4c95-b56e-2901a80720c5.png">
  
  
<img width="643" alt="image" src="https://user-images.githubusercontent.com/62703343/212582407-ad55c7dd-f9d3-4007-bed6-7cf3828af46a.png">
  
  
<img width="1198" alt="image" src="https://user-images.githubusercontent.com/62703343/212587403-00852033-bcb9-4d67-9a4b-4ec0eaa0e3a4.png">

<img width="1198" alt="image" src="https://user-images.githubusercontent.com/62703343/212587578-e5b3116a-0145-4bcc-9245-0b553830d000.png">
  
  
<img width="1198" alt="image" src="https://user-images.githubusercontent.com/62703343/212587627-dadb466c-102f-496d-be15-7d34dc6e2ba6.png">
  
  
<img width="1198" alt="image" src="https://user-images.githubusercontent.com/62703343/212587534-a250a9ce-d1c8-4dca-b10d-5730f84ba26f.png">
  
  
<img width="1480" alt="image" src="https://user-images.githubusercontent.com/62703343/212585360-eab39944-37ca-452f-8b9f-afbe6f1d005f.png">
  

<img width="1480" alt="image" src="https://user-images.githubusercontent.com/62703343/212587861-14fd3485-b3fa-42d8-9b13-d48c59451a2a.png">

  
<img width="726" alt="image" src="https://user-images.githubusercontent.com/62703343/212586923-f4af6942-5db5-4a9e-8a15-8e79b0d76288.png">
  
  
<img width="537" alt="image" src="https://user-images.githubusercontent.com/62703343/212587076-822afb79-6f0b-4e39-b54f-a537d2018169.png">
  
  
<img width="1015" alt="image" src="https://user-images.githubusercontent.com/62703343/212587247-30eddcdc-c2ff-4d52-ab33-4c5636bee6af.png">
  

<img width="906" alt="image" src="https://user-images.githubusercontent.com/62703343/212588257-870b2585-8f83-4fb3-98a5-ce88286c154d.png">


## 鸣谢下列作者的文章和项目:
大佬 Nike Jeff

## 免责声明:
* 本程序仅供学习了解, 非盈利目的，请于下载后 24 小时内删除, 不得用作任何商业用途, 文字、数据及图片均有所属版权, 如转载须注明来源。
* 使用本程序必循遵守部署免责声明。使用本程序必循遵守部署服务器所在地、所在国家和用户所在国家的法律法规, 程序作者不对使用者任何不当行为负责。
