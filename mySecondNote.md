# 代码
## 单句代码
使用反引号将其包括起来  
例如：  
 `printf()`函数  
***
## 代码区块
使用四个空格或一个Tab来表示  
例如：
 
    #include <iostream>
    using namespace std;
    int main()
    {
        cout<<"Hello, world!\n";
        system('pause');
        return 0;
    }
<font size = 5>***这里需要特别注意嗷！***</font>
***
由此看来只用四个空格或tab是没有区块效果的，如果与上一行没有多空开一行的效果会变成  
    #include <iostream>
    using namespace std;
    int main()
    {
        cout<<"Hello, world!\n";
        system('pause');
        return 0;
    }  
***

## 段代码
可用三个反引号引入一段代码，且可以规定引入代码段的语言类型以得到不同高亮效果
例如：
```javascript
$(document).ready(function () {
    alert('I am Groot.');
});
```
又如：
```python
#蟒蛇绘制
import turtle
turtle.setup(650,350,0,0)#设定窗体大小与开始位置，去掉后两位则默认在正中心
turtle.penup()#别名turtle.pu，抬起画笔，画面内为正中心(0,0)
turtle.fd(-250)#forward/fd()向正前方向运行，back/bk()向正后方向运行，circle(r,angle)以左边r位置为圆心运行angle弧度
turtle.pendown()#别名turtle.pd，落下画笔
turtle.pensize(25)#别名turtle.width
turtle.pencolor("blue")#可通过字符串（小写）或RGB小数值或元组值赋值
turtle.seth(-40)#改变当前行进的~绝对~方向 
for i in range(4):#range为次数从0到range-1，print()中的,可以看作加一个空格
    turtle.circle(40,80)
    turtle.circle(-40,80)
turtle.circle(40,80/2)
turtle.fd(40)
turtle.circle(16,180)
turtle.fd(40*2/3)
turtle.done()#运行完不会直接退出需要手动退出
```
这种情况下不用与之前行空开，即只有用Tab或空格引入代码段时需要与前一行空开。

# 链接
链接有两种显示方式，一种是显示名称，另一种是直接显示网址。
* [必应](www.bing.com)
* <https://www.baidu.com>或<www.baidu.com>，但高亮效果不同。
* VSCode中还可以直接键入网址无需符号辅助，例如 www.sina.com或https://www.google.com（在原文中的显示有所区别），但是在原文中该网址不会高亮，只会在笔记中高亮。
## 高级链接！
***
可以将此方式看作传一个引用，例如：  
> [必应][1]  
[1]: https://www.bing.com

这里我出现了问题，无法成功引用，关于Markdown的高级链接语法请点[这里](https://www.runoob.com/markdown/md-link.html)。

# 图片
语法格式为  
![代替图片的文字](图片的地址)
例如：  
![github头像](file:///C:/0931Jason/Photos/109951163701197524.jpg)
![我们从哪里来？我们是谁？我们要到哪里去](https://upload.wikimedia.org/wikipedia/commons/f/fc/Woher_kommen_wir_Wer_sind_wir_Wohin_gehen_wir.jpg)
不过为什么本地图片显示不了，一定是我又哪里出bug了，今天怎么学得这么不顺。  
因为Markdown的HTML属性，他的图片还可以使用\<img>标签标示从而控制图片的大小。  
例如：  
<img src="https://upload.wikimedia.org/wikipedia/commons/f/fc/Woher_kommen_wir_Wer_sind_wir_Wohin_gehen_wir.jpg" width="50%">

***
今天眼睛好疼，就写到这，明天看补完作业还有没有时间继续Markdown  
<img src="https://pic.38fan.com/20190326/20190326133230263864.png" width="25%">)