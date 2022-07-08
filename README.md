# 拼成语 | Chinese Wordle

<https://allanchain.github.io/chinese-wordle/>

**太长不看：** 这是一个根据声母和韵母猜成语的小游戏。 必须输入一个合法的成语。 尽量在浏览器打开，而非微信。 

##  颜色提示 

![img](public/color-explain.jpg)

 如果你猜的成语中某一个声母或韵母： 

- 位置与待猜成语相同，它就会被标成绿色
- 出现在待猜成语中但位置错误，就是黄色
- 如果在你猜的成语中多次出现而在待猜成语中只出现一次，则不会重复着色；如果都是多次出现（在待猜成语中出现 n 次），至多着色 n 次
- 韵母组合正确，会加上绿色双下划线
- 压根没出现在待猜成语中，就是灰色



##  其他提示 

 事实证明如果只有颜色的提示，猜成语会比较困难。所以游戏上方还有一栏提示，比如在简单版中： 

-  待猜成语的某个字的声母和韵母： 
  - 都被猜到过，则提示该声母韵母组合
  - 组合被猜到，则提示该字的音调
- 所猜的成语的某个字的与待猜成语相同位置的字发音相同，则提示这个字



 不同难度选择的区别也就在于这部分提示的多少和获得提示的难度。 

##  拼音 

 游戏中的拼音声母韵母划分基本按照 [ 《汉语拼音方案》 ](http://www.moe.gov.cn/jyb_sjzl/ziliao/A19/195802/t19580201_186000.html) 来进行， 有关韵母写法的问题，可翻阅新华字典附录《汉语拼音方案》韵母表后第 4 和第 5 条。 

 主要不同之处在于，这里认为 **zhi** 等里和 **ji** 等里的 **i** 是一样的。 

 感谢 [ @Yixuan-Wang ](https://github.com/Yixuan-Wang) 对拼音算法的校对修正工作。 

##  成语与参考资料 

 游戏中用作待猜成语的主要来自 [ THUOCL 的成语词频表](http://thuocl.thunlp.org/#chengyu)， 并经过人工简单筛选，去掉了一部分不适合猜的成语。 作为验证输入的成语比用作待猜成语的数量更多，其选取和注音主要来自[汉典](https://www.zdic.net/cd/cybs/)，并利用 [ pypinyin ](https://github.com/mozillazg/python-pinyin) 库作了简单的自动校对。 部分未能自动校对的一百来个成语被未被纳入列表。 

##  分享 

 可以直接截屏分享来晒本局成绩，也可在右上角的统计按钮中查看一些统计信息。 

 游戏结束后，点击复制链接按钮，邀请好友打开，即可让好友也来猜猜这个成语。 

##  项目 

 本项目[在 GitHub 开源](https://github.com/AllanChain/chinese-wordle)，如有问题和建议欢迎提出。 

 项目的灵感来自于 wordle，很容易搜到，不多叙述。 
