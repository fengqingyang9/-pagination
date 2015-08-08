# 原生JS实现的分页
#### 实现的功能
之前在做项目的时候需要一个表格插件展示数据，当时就用的是jquery datatable这个插件，但这个插件
在面对大数据的时候，虽然它提供了在服务端分页的功能，但是过于呆板不够灵活，不能适应我们项目
的需求，项目中获取数据都是利用ajax从后端来获取的。于是就有了想自己写个分页功能的打算。   <br/>
下面是我根据分页查询的思想，用原生js实现的分页功能，封装成了分页函数，可拓展性较好。

    page({
    
            id: 'div1',  //生成分页需要的id
            nowNum: 5,   //当前页
            allNum: 100, //总页数
            callBack: function (now, all) {   //回调函数    
                //now为当前页，all为总页数
                //这里可以根据当前页和总页数，通过ajax请求从后端获取数据
    
            }
    
        });


