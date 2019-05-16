###jQUERY
````javascript
//1.入口函数
$(document).ready(function() {
});

$(function() {
  
});
//2.选择器
//基本选择器  $("")
//$("#id值")；
//$(".class值")；
//$("eleName")；

//层级选择器
//$("选择器1 选择器2")；
//$("选择器1 > 选择器2")；
//$("选择器,选择器2")；
//$("eleName.select")；

//过滤（伪类）
//$("选择器1：eq(索引)")；
//$("选择器1：odd(索引)")；
//$("选择器1：even(索引)")；

//表单
//$("input:checked)；
//$("input:selected)；
//$("input:disabled)；


//筛选选择器（都是方法）
//$("选择器").first()；
//$("选择器").last()；
//可以不传递参数  获取所有子元素   传递参数获取的实当前标签对应元素
//$("选择器").children("div")；
//可以传递参数，如果传递了获取的传递参数对应的所有相邻元素
//$("选择器").siblings("div")；
//$("选择器").prev("div")；
//$("选择器").prevAll("div")；
//$("选择器").next("div")；
//$("选择器").nextAll("div")；
//获取父集元素
//$("选择器").parent()；


//3.jq对象和js对象相互是不可以调用内部的方法的
//js对象和jq对象相互转化：
//js对象转jq对象  $(jsObj);

//get();是转为一个数组  get(0);第一个元素   
//jq对象转js对象  $("div").get();  --> 数组   $("div").get(0);-->第一个元素  $("div")[索引];

//4.样式
//css
//单个样式   css("样式名"，"样式值");
// $("div").css("color","red");
//多个个样式   css({属性名：属性值，属性名：属性值，属性名：属性值..});

//class
//addClass("类名");
//removeClass("类名");
//toggleClass("类名"); 切换 


//5.属性
//index();当前元素对应索引


//6.动画
//(1）三组基本动画
//显示/隐藏/切换
//传递参数：
//slow 200ms   normal:400ms  fast600ms
//直接ms数

//第一组不传递参数没有动画效果
//show();  hide(); toggle();
//滑入/滑出、切换
//slideDown  slideUp  slideToggle();
//淡入/淡出、切换
fadeIn/fadeOut/fadeToggle 
//(2)自动义动画
//{}:改变的样式    时间：毫秒   运动方式（swing/linear）  回调函数（动画完成要做到事情）
//参数可以省略
 //jqObj.animate({},时间，运动方式，回调函数);
 //我们可以自己手动的去结束动画（结束上一次执行的动画效果）
 //stop();
 
 
 //7.循环遍历
 //each
 //(1)给原型添加循环遍历
 //(2)给实例添加的循环遍历
 //(3)隐式迭代
 
 
 //8.关于节点的操作
 
//（1）.创建节点
//传递的参数是拼接好的html节点字符串
$("<li>你好</li>");

//（2）添加
//添加到末尾
//append        父亲.append(儿子);
//appnedTo         儿子.appendTo(父亲);

//添加到开头
//prepend       父亲.prepend(儿子);
//prependTo     儿子.prependTo(父亲);
//insertAfter   把所有匹配的元素插入到另一个、指定的元素元素集合的后面。
//insertBefore  把所有匹配的元素插入到另一个、指定的元素元素集合的前面。
//empty :清空内容
// $("#myUl").empty();
//remove：删除
//$("#myUl").remove();


//attr
//一个参数 获取
//二个参数  设置

//prop:表单元素
//一个参数 获取
//二个参数  设置

//克隆参数为false:不克隆事件，参数为true克隆事件
//clone();
//获取表单元素的值
//val()


````

**`9.事件`**
>jq对象.事件名称(function(e){});
>jq对象.on("事件名称”，“代理对象”，数据，function(){});

>当前元素已经绑定了某个事件再次去触发
>>jq对象.事件();
>>jq对象.trigger("事件名称");


