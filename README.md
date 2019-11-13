# 恋爱纪念日

#### 介绍
纪念恋爱的时长

#### 软件架构
软件架构说明


#### 安装教程

先下载源代码

```bash
git clone git@github.com:Yifengzis/love.git
```

更改恋爱日期，修改index.html

```javascript
        var textAnimate = eval(Jscex.compile("async", function () {
		    var together = new Date();
		    together.setFullYear(2018,00,29); 				//时间年月日
		    together.setHours(00);					        //小时	
		    together.setMinutes(00);					    //分钟
		    together.setSeconds(00);				       	//秒前一位
		    together.setMilliseconds(00);				    //秒第二位
		    $("#code").show().typewriter();
            $("#clock-box").fadeIn(500);
            while (true) {
                timeElapse(together);
                $await(Jscex.Async.sleep(1000));
            }
        }));
```
