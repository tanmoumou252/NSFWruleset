[🍞English version](https://github.com/tanmoumou252/NSFWruleset#english-version) |[🍘中文版本](https://github.com/tanmoumou252/NSFWruleset#%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87%E7%89%88%E6%9C%AC) 

# English version
Some triage rules `rule-set` for NSFW-website.It adapted to [Akasha Terminal clash](https://github.com/MetaCubeX/mihomo), and can be used in custom local profiles, see the anchor references [documentation](https://wiki.metacubex.one/config/syntax/#_6) for simplification. 

`&` anchor and `*` alias, can be used to reference, `&` used to create the anchor, `<<` that merge to the current data, `*` used to reference anchor 

```yaml
p: &p
  type: http
  interval: 3600
  health-check:
    enable: true
    url: https://www.gstatic.com/generate_204
    interval: 300

proxy-providers:
  provider1:
    <<: *p
    url: ""
    path: ./proxy_providers/provider1.yaml

  provider2:
    <<: *p
    type: file
    path: ./proxy_providers/provider2.yaml
```

I also have a few local profiles in my repository, with Chinese comments, the local profile is basically compatible with each client's clash core, no matter if it's a router or an Android or a computer.

 I'm new here,and still learning how it work.   
 I put this on github to optimize the use of local profile which you can get from [hope140](https://github.com/hope140/Clash) and [I](https://raw.githubusercontent.com/tanmoumou252/NSFWruleset/main/8%E5%88%86%E7%BB%84%E6%9C%AC%E5%9C%B0%E9%85%8D%E7%BD%AE-%E5%A1%AB%E8%AE%A2%E9%98%85.yml).  
## how to use
1. Create a new provider under `rule-providers`, and fill in the url with the address of [NSFW.yaml](https://raw.githubusercontent.com/tanmoumou252/NSFWruleset/main/NSFW.yaml).  eg.  
![图片](https://user-images.githubusercontent.com/118299342/202003750-87bc9bf9-7e5b-4da6-84ef-4de59b5f8c31.png)  
I`m your provider now.  
2. Scroll to rules and add `- RULE-SET, NSFW, proxy groups you set`, as shown in the picture.  
![图片](https://user-images.githubusercontent.com/118299342/202005614-a1ca3c3a-f142-4357-add5-fe71ba779667.png)     
3. Now go to update your local profile, if no error is reported, you can start your journey of nsfw.  
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
The $\color{#FF0000}{NSFW}$ case in the above code is not the same, and it will report an error.    
## others  
* This English document is written by Google Translate and DeepL Translate.  
* As we all know,most of the people who use clash, they speak Ch\**ese.People in other places rarely use such tools, of course we know that parts of the US restrict tiktok, Iran controls it even more, it's like Ch\**a all over again, if you ask me. Others just use it because Netflix Disney doesn't have the rights to a TV show or movie in their area.   
* In other words, I don’t really need to write English documents, and now the function of translating web pages is so developed.  
* Whatever，hope u like that.  

------  
# 简体中文版本
一些适配[虚空终端 clash](https://github.com/MetaCubeX/mihomo)的"你懂的"网页的分流规则`rule-set`,可以在本地配置中使用,要简化可以参看锚点引用[文档](https://wiki.metacubex.one/config/syntax/#_6)  

`&` 锚点和 `*` 别名,可以用来引用,`&` 用来建立锚点,`<<`表示合并到当前数据, `*` 用来引用锚点 
```yaml
p: &p
  type: http
  interval: 3600
  health-check:
    enable: true
    url: https://www.gstatic.com/generate_204
    interval: 300

proxy-providers:
  provider1:
    <<: *p
    url: ""
    path: ./proxy_providers/provider1.yaml

  provider2:
    <<: *p
    type: file
    path: ./proxy_providers/provider2.yaml
```
我的仓库里也有几个本地配置模板,带中文注释,本地配置基本上各个客户端的clash核心都兼容,不管是路由器的还是安卓的或是电脑的 

初来乍到，还在学习如何去使用github 

因为[hope140](https://github.com/hope140/Clash)给到的`rule-set`预设中对~~NSFW~~的网页照顾不到,于是萌生了照猫画虎的想法,干脆将我收藏夹里的好东西全都做成规则发到项目里  

## 使用方法  
1. 在rule-providers下新建一个服务商，在服务商的url里填上这份[NSFW.yaml](https://raw.githubusercontent.com/tanmoumou252/NSFWruleset/main/NSFW.yaml)的地址,就像这个图片这样  
![图片](https://user-images.githubusercontent.com/118299342/202003750-87bc9bf9-7e5b-4da6-84ef-4de59b5f8c31.png)  
好的那么现在我是你的规则服务商了  
2. 在rules这里，添加`- RULE-SET,NSFW,你设置的proxy-groups`，就像图片这样  
![图片](https://user-images.githubusercontent.com/118299342/202005614-a1ca3c3a-f142-4357-add5-fe71ba779667.png)  
3. 现在去刷新|更新你的本地配置没有报错，那么就可以开始上路了  
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
上面这段代码 $\color{#FF0000}{NSFW}$ 大小写就不一样，就会报错  

## 其他
不论如何，希望它能帮到你的忙  

