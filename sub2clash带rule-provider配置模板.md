# sub2clash带```rule-provider```配置模板
## sub2clash中,```rule-provider```需要手动填写多次
*比如说下面这张图*

![图片](https://github.com/tanmoumou252/NSFWruleset/assets/118299342/2d72357c-9625-443b-b53d-da55f5d6d4c9)

**那么在此提供一个解析链,用于直接填写上图的内容,你可以进行二次更改,这些```rule-provider```来自GitHub**

**你的clash或许无法访问GitHub,那么会造成:因为无法获得```rule-provider```而导致clash无法启动/配置无法切换的问题**

```http
http://localhost:8011/clash?sub=https%3A%2F%2F%E8%AE%A2%E9%98%85%E9%93%BE%E6%8E%A5%23%F0%9F%92%B5&refresh=true&autoTest=true&lazy=true&nodeList=false&ruleProvider=%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Ftanmoumou252%2FNSFWruleset%2Fmain%2FNSFW.yaml%2C%F0%9F%8E%AF%20R18%2Ctrue%2CNSFW%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Ftanmoumou252%2FNSFWruleset%2Fmain%2FLan_CN.yaml%2CDIRECT%2Ctrue%2CLan_CN%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FGoogle%2FGoogle.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CGoogle%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FGoogleDrive%2FGoogleDrive.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CGoogleDrive%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FOneDrive%2FOneDrive.yaml%2CDIRECT%2Cfalse%2COneDrive%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FMicrosoft%2FMicrosoft.yaml%2CDIRECT%2Cfalse%2CMicrosoft%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FApple%2FApple.yaml%2CDIRECT%2Cfalse%2CApple%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FTelegram%2FTelegram.yaml%2C%F0%9F%93%B2%20%E7%94%B5%E6%8A%A5%E6%B6%88%E6%81%AF%2Cfalse%2CTelegram%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FYouTube%2FYouTube.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CYouTube%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FBahamut%2FBahamut.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CBahamut%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FGlobalMedia%2FGlobalMedia.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CGlobalMedia%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FBiliBili%2FBiliBili.yaml%2CDIRECT%2Cfalse%2CBiliBili%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FChinaMedia%2FChinaMedia.yaml%2CDIRECT%2Cfalse%2CChinaMedia%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FDeveloper%2FDeveloper.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CDeveloper%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Ftanmoumou252%2Ffirefoxruleset%2Fmain%2FFirefox.yaml%2CDIRECT%2Cfalse%2CFirefox%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FGitHub%2FGitHub.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CGithub%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Ftanmoumou252%2FNSFWruleset%2Fmain%2FGPT_AI.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CGPT_AI%5D&rule=&sort=sizedesc&remove=%E5%A6%82%E6%97%A0%E6%B3%95%7C%E7%BD%91%7C%E6%B5%81%E9%87%8F%7C%E6%97%B6&replace=%5B%3C%E2%9A%9C%EF%B8%8F%3E%2C%3C%3E%5D%2C%5B%3C%E3%80%90A%E3%80%91%3E%2C%3C%3E%5D%2C%5B%3CLv1%20%3E%2C%3C%3E%5D%2C%5B%3C%20%3E%2C%3C%3E%5D
```
**URL 编码及解码```(转义)```结果为:**
```
http://localhost:8011/clash?sub=https://订阅链接#💵&refresh=true&autoTest=true&lazy=true&nodeList=false&ruleProvider=[classical,https://raw.githubusercontent.com/tanmoumou252/NSFWruleset/main/NSFW.yaml,🎯 R18,true,NSFW],[classical,https://raw.githubusercontent.com/tanmoumou252/NSFWruleset/main/Lan_CN.yaml,DIRECT,true,Lan_CN],[classical,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/Google/Google.yaml,🚀 手动切换,false,Google],[classical,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/GoogleDrive/GoogleDrive.yaml,🚀 手动切换,false,GoogleDrive],[classical,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/OneDrive/OneDrive.yaml,DIRECT,false,OneDrive],[classical,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/Microsoft/Microsoft.yaml,DIRECT,false,Microsoft],[classical,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/Apple/Apple.yaml,DIRECT,false,Apple],[classical,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/Telegram/Telegram.yaml,📲 电报消息,false,Telegram],[classical,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/YouTube/YouTube.yaml,🚀 手动切换,false,YouTube],[classical,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/Bahamut/Bahamut.yaml,🚀 手动切换,false,Bahamut],[classical,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/GlobalMedia/GlobalMedia.yaml,🚀 手动切换,false,GlobalMedia],[classical,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/BiliBili/BiliBili.yaml,DIRECT,false,BiliBili],[classical,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/ChinaMedia/ChinaMedia.yaml,DIRECT,false,ChinaMedia],[classical,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/Developer/Developer.yaml,🚀 手动切换,false,Developer],[classical,https://raw.githubusercontent.com/tanmoumou252/firefoxruleset/main/Firefox.yaml,DIRECT,false,Firefox],[classical,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Clash/GitHub/GitHub.yaml,🚀 手动切换,false,Github],[classical,https://raw.githubusercontent.com/tanmoumou252/NSFWruleset/main/GPT_AI.yaml,🚀 手动切换,false,GPT_AI]&rule=&sort=sizedesc&remove=如无法|网|流量|时&replace=[<⚜️>,<>],[<【A】>,<>],[<Lv1 >,<>],[< >,<>]
```

## GitHub给这段超长代码的右下角添加了两个正方形叠加在一起的按钮,点击即可复制
*也可以使用这个*
[***右击复制链接***](http://localhost:8011/clash?sub=https%3A%2F%2F%E8%AE%A2%E9%98%85%E9%93%BE%E6%8E%A5%23%F0%9F%92%B5&refresh=true&autoTest=true&lazy=true&nodeList=false&ruleProvider=%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Ftanmoumou252%2FNSFWruleset%2Fmain%2FNSFW.yaml%2C%F0%9F%8E%AF%20R18%2Ctrue%2CNSFW%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Ftanmoumou252%2FNSFWruleset%2Fmain%2FLan_CN.yaml%2CDIRECT%2Ctrue%2CLan_CN%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FGoogle%2FGoogle.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CGoogle%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FGoogleDrive%2FGoogleDrive.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CGoogleDrive%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FOneDrive%2FOneDrive.yaml%2CDIRECT%2Cfalse%2COneDrive%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FMicrosoft%2FMicrosoft.yaml%2CDIRECT%2Cfalse%2CMicrosoft%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FApple%2FApple.yaml%2CDIRECT%2Cfalse%2CApple%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FTelegram%2FTelegram.yaml%2C%F0%9F%93%B2%20%E7%94%B5%E6%8A%A5%E6%B6%88%E6%81%AF%2Cfalse%2CTelegram%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FYouTube%2FYouTube.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CYouTube%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FBahamut%2FBahamut.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CBahamut%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FGlobalMedia%2FGlobalMedia.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CGlobalMedia%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FBiliBili%2FBiliBili.yaml%2CDIRECT%2Cfalse%2CBiliBili%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FChinaMedia%2FChinaMedia.yaml%2CDIRECT%2Cfalse%2CChinaMedia%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FDeveloper%2FDeveloper.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CDeveloper%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Ftanmoumou252%2Ffirefoxruleset%2Fmain%2FFirefox.yaml%2CDIRECT%2Cfalse%2CFirefox%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Fblackmatrix7%2Fios_rule_script%2Fmaster%2Frule%2FClash%2FGitHub%2FGitHub.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CGithub%5D%2C%5Bclassical%2Chttps%3A%2F%2Fraw.githubusercontent.com%2Ftanmoumou252%2FNSFWruleset%2Fmain%2FGPT_AI.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CGPT_AI%5D&rule=&sort=sizedesc&remove=%E5%A6%82%E6%97%A0%E6%B3%95%7C%E7%BD%91%7C%E6%B5%81%E9%87%8F%7C%E6%97%B6&replace=%5B%3C%E2%9A%9C%EF%B8%8F%3E%2C%3C%3E%5D%2C%5B%3C%E3%80%90A%E3%80%91%3E%2C%3C%3E%5D%2C%5B%3CLv1%20%3E%2C%3C%3E%5D%2C%5B%3C%20%3E%2C%3C%3E%5D)

## ```转义```后的url人类可读,可以依据此进行url的快速搜索和批量替换
鉴于GitHub的访问不稳定,可改链接为[***cdn.jsdelivr.net***](https://www.jsdelivr.com/documentation#id-github)

[***右击复制```rule-provider```改为cdn链接的解析链***](http://localhost:8011/clash?sub=https%3A%2F%2F%E8%AE%A2%E9%98%85%E9%93%BE%E6%8E%A5%23%F0%9F%92%B5&refresh=true&autoTest=true&lazy=true&nodeList=false&ruleProvider=%5Bclassical%2Chttps%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Ftanmoumou252%2FNSFWruleset%2FNSFW.yaml%2C%F0%9F%8E%AF%20R18%2Ctrue%2CNSFW%5D%2C%5Bclassical%2Chttps%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Ftanmoumou252%2FNSFWruleset%2FLan_CN.yaml%2CDIRECT%2Ctrue%2CLan_CN%5D%2C%5Bclassical%2Chttps%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fblackmatrix7%2Fios_rule_script%2Frule%2FClash%2FGoogle%2FGoogle.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CGoogle%5D%2C%5Bclassical%2Chttps%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fblackmatrix7%2Fios_rule_script%2Frule%2FClash%2FGoogleDrive%2FGoogleDrive.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CGoogleDrive%5D%2C%5Bclassical%2Chttps%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fblackmatrix7%2Fios_rule_script%2Frule%2FClash%2FOneDrive%2FOneDrive.yaml%2CDIRECT%2Cfalse%2COneDrive%5D%2C%5Bclassical%2Chttps%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fblackmatrix7%2Fios_rule_script%2Frule%2FClash%2FMicrosoft%2FMicrosoft.yaml%2CDIRECT%2Cfalse%2CMicrosoft%5D%2C%5Bclassical%2Chttps%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fblackmatrix7%2Fios_rule_script%2Frule%2FClash%2FApple%2FApple.yaml%2CDIRECT%2Cfalse%2CApple%5D%2C%5Bclassical%2Chttps%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fblackmatrix7%2Fios_rule_script%2Frule%2FClash%2FTelegram%2FTelegram.yaml%2C%F0%9F%93%B2%20%E7%94%B5%E6%8A%A5%E6%B6%88%E6%81%AF%2Cfalse%2CTelegram%5D%2C%5Bclassical%2Chttps%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fblackmatrix7%2Fios_rule_script%2Frule%2FClash%2FYouTube%2FYouTube.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CYouTube%5D%2C%5Bclassical%2Chttps%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fblackmatrix7%2Fios_rule_script%2Frule%2FClash%2FBahamut%2FBahamut.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CBahamut%5D%2C%5Bclassical%2Chttps%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fblackmatrix7%2Fios_rule_script%2Frule%2FClash%2FGlobalMedia%2FGlobalMedia.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CGlobalMedia%5D%2C%5Bclassical%2Chttps%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fblackmatrix7%2Fios_rule_script%2Frule%2FClash%2FBiliBili%2FBiliBili.yaml%2CDIRECT%2Cfalse%2CBiliBili%5D%2C%5Bclassical%2Chttps%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fblackmatrix7%2Fios_rule_script%2Frule%2FClash%2FChinaMedia%2FChinaMedia.yaml%2CDIRECT%2Cfalse%2CChinaMedia%5D%2C%5Bclassical%2Chttps%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fblackmatrix7%2Fios_rule_script%2Frule%2FClash%2FDeveloper%2FDeveloper.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CDeveloper%5D%2C%5Bclassical%2Chttps%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Ftanmoumou252%2Ffirefoxruleset%2FFirefox.yaml%2CDIRECT%2Cfalse%2CFirefox%5D%2C%5Bclassical%2Chttps%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Fblackmatrix7%2Fios_rule_script%2Frule%2FClash%2FGitHub%2FGitHub.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CGithub%5D%2C%5Bclassical%2Chttps%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2Ftanmoumou252%2FNSFWruleset%2FGPT_AI.yaml%2C%F0%9F%9A%80%20%E6%89%8B%E5%8A%A8%E5%88%87%E6%8D%A2%2Cfalse%2CGPT_AI%5D&rule=&sort=sizedesc&remove=%E5%A6%82%E6%97%A0%E6%B3%95%7C%E7%BD%91%7C%E6%B5%81%E9%87%8F%7C%E6%97%B6&replace=%5B%3C%E2%9A%9C%EF%B8%8F%3E%2C%3C%3E%5D%2C%5B%3C%E3%80%90A%E3%80%91%3E%2C%3C%3E%5D%2C%5B%3CLv1%20%3E%2C%3C%3E%5D%2C%5B%3C%20%3E%2C%3C%3E%5D)

```转义```的时候,取消`%26 > &` `%3D > =`的```转义```,这样```转义```回来的链接sub2clash才能重新读取
> [!IMPORTANT]
> - 这段解析链还提供了几个已填写的信息
> - 在某一个订阅的所有节点前增加💵 美刀标志 - 即节点名重命名
> - 带了几个节点名替换正则表达式 - 即节点名重命名
> - ```rule-set```文件下载下来的路径是sub2clash生成的

# 以下为sub2clash模板本身

```yaml
port: 7890
socks-port: 7891
allow-lan: true
mode: Rule
log-level: info
proxies:
proxy-groups:
    - name: "🚀 手动切换"
      type: select
      proxies: 
        - <all>           
    - name: "🐟 漏网之鱼"
      type: select
      proxies:
        - DIRECT
        - "🚀 手动切换"
    - name: "🎯 R18"
      type: select
      proxies:        
        - "🚀 手动切换"
        - R18-台湾
        - R18-新加坡
        - R18-日本
        - R18-美国
    - name: "📲 电报消息"
      type: select
      proxies:
        - "🔯 故障转移"
        - "🚀 手动切换"
    - name: "🔯 故障转移"
      type: url-test
      proxies:
        - <tw>
        - <sg>
        - <jp>              #  - <countries> | - <all>
      url: http://www.gstatic.com/generate_204
      interval: 300
      tolerance: 50
    - name: "R18-台湾"
      type: url-test
      proxies:
        - <tw>
      url: http://www.gstatic.com/generate_204
      interval: 300
      tolerance: 50
    - name: "R18-新加坡"
      type: url-test
      proxies:
        - <sg>
      url: http://www.gstatic.com/generate_204
      interval: 300
      tolerance: 50            
    - name: "R18-日本"
      type: url-test
      proxies:
        - <jp>             
      url: http://www.gstatic.com/generate_204
      interval: 300
      tolerance: 50
    - name: "R18-美国"
      type: url-test
      proxies:
        - <us>           
      url: http://www.gstatic.com/generate_204
      interval: 300
      tolerance: 50

rules:
  - MATCH,🐟 漏网之鱼

```
## [yacd](https://github.com/haishanh/yacd) 中的```rule-provider```使用效果
![图片](https://github.com/tanmoumou252/NSFWruleset/assets/118299342/3f03703b-7561-4c08-9f26-965660f65749)

