third reset.css
=====

-第一：需要收集所有使用到的html标签，当然在使用标签时尽量使用不常见的标签。

-第二：基本上所有的属性都需要重置，啊啊啊，这个能穷举的完吗？经验有限，请大家多多批评，欢迎补刀，欢迎拍砖。

-第三：需要注意reset里面的优先级，需要尽量的高，这样才能覆盖用户网站的优先级。建议用id+标签的形式(ps:id定义时当然需要定义成稍显复杂点的啦)。但是不能太高哟，太高一旦高过后面渲染时想要的效果时咋办(ps:后面绘制dom时可以再提高个优先级，譬如id+class+标签)？
