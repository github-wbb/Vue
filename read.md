### 1. Vue2生命周期

含义：初始化一个vue实例，从创建到销毁的一个过程，包含不同阶段的，针对其特性，根据业务场景进行操作。

> 这些钩子函数包含初始化init(), beforeCreated() 创建dom之前，这时this，包含data还未获取到
创建之后，Dom渲染之前，渲染之后，更新，销毁等等。 
    new Vue({})
    
    init() => 
    beforeCreate => created() => 
    beforeMount => mounted() => 
    beforeUpdate() => updated() => 
    beforeDestroy() => destroyed()



### 2. Vue编码风格

2.1 组件名最好使用多个英文名 如<nav-list></nav-list>

2.2 props定义时需加类型

    props: {
        listData: {
            type: Array,
            default () {
                return []
            }
        }
    }
    
2.3 指义缩写