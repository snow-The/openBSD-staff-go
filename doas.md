# [doas](https://man.openbsd.org/doas)
## 第一眼
### 感覺
有看沒有懂，感覺像用另外一個身份執行這個命令
### 生難字
#### style
我對於style的定義感到模糊，用英文直接翻譯是風格，但手冊給我的感覺不像。
#### mandatory
什麽是强制性的，對其意義感受到不明白
#### umask
這個是什麽
## 研究了一下
### 作用
就是用另外一個身份執行命令，并且使用該用戶的文件目錄從home一路衍生。需要該用戶的密碼，并且記錄也會是以該用戶的名字。
### 生難字匯大調查
#### style
給你的身份添加各種權限和限制，詳細要看[login.conf.5](https://man.openbsd.org/login.conf.5)
#### madatory
還是不明白
#### umask
大概的作用就是讓你的記錄名字也是那個用戶
### 注意
-u 是默認root權限啊！
## 持續的問題
command [args]是什麽
## 實戰
### 過程
看著[paranoid.life](https://youtu.be/dsW486DcBLU)的影片一起做，結果看不懂。
看了jrmu提供的IRCnow[上面的内容](https://wiki.ircnow.org/?n=Doas.Configure)
就懂了，還發現了doas -s可以持續使用。
### 結尾
因爲目前只有我一個用戶所以說還是有一些功能無法實作..
之後再回來吧
