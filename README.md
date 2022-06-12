vue-
====

# vue day01
>>想让vue工作就必须创建一个Vue实例，且要传入一个配置对象
>>root容器中的代码依然符合html规范，只是混入了一些vue语法
>>容器中的代码被称为【vue模板】
>>真实的开发中只有一个vue实例，并且会配合组件一起使用
>>{{xxx}}中的xxx要写js表达式，且xxx可以自动读取到data中的所有属性
>>一旦data中的数据发生改变，那么模板中要那个到该数据的地方也会自动更新
(```html
    <div id=" root">
        <h1>hello {{name}}{{address}}{{Date.now()}}</h1>
    </div>
    ```)
(```javascript
<script>
        Vue.config.productionTip = false
        new Vue({
            el: '#root',
            data: {
                name: 'world',
                address: '北京'
            }
        })
    </script>
```)
>>
