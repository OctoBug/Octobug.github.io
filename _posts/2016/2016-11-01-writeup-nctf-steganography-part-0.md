---
layout: post
title: NCTF 隐写术 3 题题解
tags: NCTF Write-up Steganography
---

* 目录: 
{:toc}

### 50 女神 
* 题目:  
![](http://r.photo.store.qq.com/psb?/V11aPCg53lyBwf/UhLwVOZFh*rleRbZcYOeg00p9yK9gXlhOceSvc6Xe08!/r/dAkBAAAAAAAA){: width="80%"}  
	
	> 听说这是女神的私房照，里面藏着flag哦  
	> [http://115.28.150.176/misc1.jpg](http://115.28.150.176/misc1.jpg)  

* 题解:  
分值这么低, 正常思路是解压成rar, 或者直接看二进制内容. 将图片另存到本地, 用记事本打开图片, 搜nctf: 
![](http://r.photo.store.qq.com/psb?/V11aPCg53lyBwf/eL3UfGlFbcT60bvzKPgxLKCO0WztgKo8xvYkc91pTns!/r/dHABAAAAAAAA){: width="100%"}

* flag: nctf{pic_yin_xie_shu}
<hr>

### 100 图种 
* 题目:  
![](http://r.photo.store.qq.com/psb?/V11aPCg53lyBwf/mYQuGheyAxU3tpkvg8pksi7.ltnKHMTvFjCkq0qtofM!/r/dNwAAAAAAAAA){: width="80%"}  
	
	> flag是动态图最后一句话的拼音首字母  
	> 加上nctf{}  
	> ![](http://ctf.nuptsast.com/static/uploads/1cf33bb62640e61a1a5e3892cb348b04/555.gif)  

* 题解:  
1. gif 下载下来, 用 winhex 打开, 拉到最下面, 发现 ZIP 文件头 `PK...`:  
![](http://r.photo.store.qq.com/psb?/V11aPCg53lyBwf/rj1YXvgC.ipLscBQ1BYhXMBBcbbKY5nGLybRbilKXXA!/r/dI8AAAAAAAAA){: width="80%"}  
2. 将 gif 后缀改为 zip, 解压得到另一张有文字的 gif, 用 Ulead GIF Animator 打开, 最后一帧最后一句话的首字母即是 flag:
![](http://r.photo.store.qq.com/psb?/V11aPCg53lyBwf/ZfprmyiGnS.V8v1thae8b8D7YbBDr5PJE79LP9j2hdU!/r/dNwAAAAAAAAA){: width="80%"} 

* flag: nctf{dssdcmlw}
<hr>

### 400 丘比龙De女神 