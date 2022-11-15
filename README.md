# English version
NSFW-website-rule-for-Clash (Actually it is [CFW](https://github.com/Fndroid/clash_for_windows_pkg),not the [Clash](https://github.com/Dreamacro/clash))   
 I'm new here,and still learning how it work   
 I put this on github to optimize the use of [localprofile](https://docs.cfw.lbyczf.com/contents/parser.html#%E5%90%91%E6%9C%AC%E5%9C%B0%E9%85%8D%E7%BD%AE%E6%96%87%E4%BB%B6%E6%B7%BB%E5%8A%A0%E8%AE%A2%E9%98%85%E4%BF%A1%E6%81%AF) which you can get from [hope140](https://github.com/hope140/Clash)  
 ## how to use
1. Create a new provider under `rule-providers`, and fill in the url with the address of [NSFW.yaml](https://raw.githubusercontent.com/tanmoumou252/NSFW-website-rule-for-Clash/main/NSFW.yaml).  eg.  
  
![图片](https://user-images.githubusercontent.com/118299342/202003750-87bc9bf9-7e5b-4da6-84ef-4de59b5f8c31.png)  
  
I`m your provider now  

2. Scroll down to rules and add `- RULE-SET, NSFW, proxy groups you set`, as shown in the picture  
  
  ![图片](https://user-images.githubusercontent.com/118299342/202005614-a1ca3c3a-f142-4357-add5-fe71ba779667.png)  
    
3. Now go to [CFW](https://github.com/Fndroid/clash_for_windows_pkg) to update your [localprofile](https://docs.cfw.lbyczf.com/contents/parser.html#%E5%90%91%E6%9C%AC%E5%9C%B0%E9%85%8D%E7%BD%AE%E6%96%87%E4%BB%B6%E6%B7%BB%E5%8A%A0%E8%AE%A2%E9%98%85%E4%BF%A1%E6%81%AF) or Parsers. If no error is reported, you can start your journey of nsfw  
## attention  
* The yaml grammar pays great attention to basic ___alignment___. You can check whether there is a ___space___ after the colon of the line of code that reports the error.
* Besides,___case sensitive___,eg. 
```  
rule-providers:  
  NSFW:  #here are some capital letters
    type: http  
    behavior: classical  
    path: ./RuleSet/NSFW.yaml  
    url: https://raw.githubusercontent.com/tanmoumou252/NSFW-website-rule-for-Clash/main/NSFW.yaml  
    interval: 86400  

rules:  
  - RULE-SET,nsfw,🌍 GlobalMedia  #here are some lowercase letters
```  
The above code has different letter sizes, and an error will be reported  
  
## others
This English document is written by Google Translate and Baidu Translate  
As we all know,most of the people who use clash, they speak Chinese.People who speak other languages rarely need to use this tool, unless they are also here, or company routing restricts web access  
In other words, I don’t really need to write English documents, and now the function of translating web pages is so developed  
Whatever，hope u like that  
 
  
------
  
# 简体中文版本
一些“你懂的”网页在[clash for win](https://github.com/Fndroid/clash_for_windows_pkg)[本地配置](https://docs.cfw.lbyczf.com/contents/parser.html#%E5%90%91%E6%9C%AC%E5%9C%B0%E9%85%8D%E7%BD%AE%E6%96%87%E4%BB%B6%E6%B7%BB%E5%8A%A0%E8%AE%A2%E9%98%85%E4%BF%A1%E6%81%AF)中使用的分流规则  
初来乍到，还在学习如何去使用github  
该项目是为了在[本地配置](https://docs.cfw.lbyczf.com/contents/parser.html#%E5%90%91%E6%9C%AC%E5%9C%B0%E9%85%8D%E7%BD%AE%E6%96%87%E4%BB%B6%E6%B7%BB%E5%8A%A0%E8%AE%A2%E9%98%85%E4%BF%A1%E6%81%AF)里用的，因为[hope140](https://github.com/hope140/Clash)给到的ruleset预设中对~~NSFW~~有些网页照顾不到。其他地方(指除了本地配置以外)也可以用到  
并且我不想手动添加那几个网页的规则到本地文件里，于是萌生了照猫画虎的想法，干脆将我收藏夹里的好东西全都做成规则发到项目里  
## 使用方法  
1. 在rule-providers下新建一个服务商，在服务商的url里填上这份[NSFW.yaml](https://raw.githubusercontent.com/tanmoumou252/NSFW-website-rule-for-Clash/main/NSFW.yaml)的地址,就像这个图片这样  
![图片](https://user-images.githubusercontent.com/118299342/202003750-87bc9bf9-7e5b-4da6-84ef-4de59b5f8c31.png)  

好的那么现在我是你的规则服务商了  
2. 往下翻到rules这里，添加`- RULE-SET,NSFW,你设置的proxy-groups`，就像图片这样  
![图片](https://user-images.githubusercontent.com/118299342/202005614-a1ca3c3a-f142-4357-add5-fe71ba779667.png)  
3. 现在去CFW更新你的本地配置或者预处理配置，没有报错，那么就可以开始上路了  

## 注意事项  
* yaml语法很注重基本的空格，或者应该说对齐，有报错很可能是你没对齐，报错那一行的冒号后面可以检查下是不是有空格  
* 以及，大小写要统一，比如  
```  
rule-providers:  
  NSFW:  #这儿的nsfw是大写
    type: http  
    behavior: classical  
    path: ./RuleSet/NSFW.yaml  
    url: https://raw.githubusercontent.com/tanmoumou252/NSFW-website-rule-for-Clash/main/NSFW.yaml  
    interval: 86400  

rules:  
  - RULE-SET,nsfw,🌍 国外媒体  #这儿的nsfw是小写
```  
上面这段代码nsfw大小写就不一样，就会报错
## 其他
不论如何，希望它能帮到你的忙  

