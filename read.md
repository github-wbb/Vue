1. Vue2生命周期

含义：初始化一个vue实例，从创建到销毁的一个过程，包含不同阶段的，针对其特性，根据业务场景进行操作。

new Vue({})

init() => beforeCreate => created() => beforeMount => mounted() => beforeUpdate() => updated() => beforeDestroy() => destroyed()

这些钩子函数包含初始化init(), beforeCreated() [创建dom之前，这时this，包含data还未获取到]
创建之后，Dom渲染之前，渲染之后，更新，销毁等等。 