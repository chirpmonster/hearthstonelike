<h2>2020.5.19</h2>
1.解决了一个bug：php返回多个JSON对象会是{}{}{}的形式，通过服务端echo json_encode($row);echo "!";客户端let data=res.data.split('!');完美解决
<br>
2.成功将卡牌数据放在MYSQL里，产生了一个bug是第一次初始化随即卡牌的时候由于是异步，导致随即失败，已修复，又产生有时候卡牌不显示的bug，正在调试问题
<br>
3.2问题解决，原因是忘记初始化数组
<h2>2020.5.18</h2>
1.花了一天时间装好了MYSQL和PHP环境，并且一步一步跟着网上的教程完成前端Axios连接PHP，PHP连接MYSQL，明天就可以修改我的程序了：
PHP从MYSQL获取内容返回JSON
<br>
2.域名审核完了，挺快的，把域名和服务器连接了，域名可以直接访问网站http://yingyingguai.club
<br>
3.计划：正在学node.js，计划使用路由简化链接
<h2>2020.5.14</h2>
1.提前随机卡牌的时间，防止翻开卡牌的时候还没加载完！
<h2>2020.5.13</h2>
1.云服务器使用成功!
<br>
http://139.196.137.150
<br>
2.修复了一个css的bug，原因是橙卡我命名为gold，金币也命名为gold，所以有一个显示小bug
<br>
3.化了作弊的体验(各种意义上)
<br>
4.给每个界面添加loading
<h2>2020.5.12</h2>
1.研究云服务器
<h2>2020.5.10</h2>
1.为了做一个翻面效果做出来一个接一个的bug（处理了好久），最奇怪的是transform-style:preserve-3d的bug...
<br>
2.导入了一个拓展包135张卡，用对象数组的形式，有空改成JSON的形式，感觉更规范一点吧
<br>
3.作弊模式
<br>
4.添加开包音效
<br>
5.修复收藏界面完成按钮返回的bug
<br>
6.添加一个音频的队列，防止连续翻开多张卡的时候音效覆盖掉
<br>
7.Vue的mounted只能同时生效一个，暂时不知道如何解决
<br>
8.连续播放音效会有一个灰色的条子，不知道是什么
<br>
9.优化手机端的体验
<h2>2020.5.9</h2>
1.今天课少，肝了好久..没想到一个css动画用了那么久
<br>
由于transform-style:preserve-3d导致旋转过程有显示bug..删掉就好了
<br>
data里数组的操作也弄了很久，浅拷贝解决问题
<br>
明天把随机的逻辑和音效写好就ok了
<br>
2.优化空格键事件，阶段、间隔等
<h2>2020.5.8</h2>
1.卡包页面和JS逻辑制作完成（拖动效果，背景<video>），明天用CSS制作开包动画
<br>
2.添加空格键开包监听
<br>
3.设置切换网页之间的延时，正常播放点击音效
<br>
遇到问题：
<br>
1.切换音频视频用v-bind写无法正常切换，用jQuery写没问题
<br>
2.Vue之间无法传输数据（卡包数量）
<h2>2020.5.7</h2>
1.完善主页面的absolute定位
<br>
2.添加点击音效
<br>
3.制作开包页面
<h2>2020.5.1</h2>
1.解决之前的冒泡问题
<h2>2020.4.29</h2>
1.优化loading界面
<br>
2.添加主页面监听esc
<h2>2020.4.26</h2>
主页面交互完成
<h2>2020.4.25</h2>
制作静态主页面
<h2>2020.4.24</h2>
1.添加音频
<br>
2.loading界面
<h2>2020.4.23</h2>
闲的时候发现了两个bug，已解决
<br>
1.卡牌移动时的z-index问题
<br>
2.窗口模式下的错位问题（通过JS定位解决）
<h2>2020.4.21</h2>
暂时告一段落吧，先去学习一下es6,webpack,协议,安全,然后再回来肝完这个项目。
<br>
目前只做完了“收藏”的一部分，目前没有任何bug，有几个未解决的问题用了另一种方法解决
<br>
问题1：如何除了一个div之外全部模糊？我查阅了一些资料，都没有能解决这个问题，于是我把那个不模糊的div拿到的最外面..算是变相解决了
<br>
问题2：阻止冒泡（vue中的.stop修饰符，return false，e.stopPropagation()都尝试过了，无效，原因未知），最后添加了一个变量isdeleting来阻止父元素的click事件-->已解决,.stop可以解决问题，之前失败应该是缓存问题
<br>
未来完善项目的打算：
<br>
1.翻页（用css3动画）
<br>
2.新建卡组
<br>
3.编辑卡组
<br>
4.卡组命名
<br>
5.JSON存储卡牌信息
<br>
6.导入很多很多卡牌
<br>
7.完善筛选法力值
<br>
8.制作卡牌与高级筛选
<br>
完成上述内容后，制作主页面和战斗页面（有生之年？）
<br>
加油！奥利给！
