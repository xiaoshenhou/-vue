<template>
<!-- 这里面写DOM结构 -->
     <div>
            <h2>学校名字：{{Xname}}</h2>
            <h2>学校地址：{{Xaddress}}</h2>
            <Student></Student>
     </div>
</template>


<script>
     import Student from './Student.vue'
// 组件交互相关的代码(数据、方法、等等)
       const School = {
            data(){
                 return {
                      Xaddress:"河南省新乡是长垣县",
                    Xname:"长垣一中"
                }
            },
            components:{
                 Student:Student
            }
        }
     export {School}
// 最终整个文件要暴露在外部，说白了也就是得有一个输出的代码，让别的文件可以输入
// 如何暴露呢？有三种方法
//     1.export {组件名}    统一暴露
//     2.在每一个要暴露的定义的变量前加一个export    这叫分别暴露
//     3.export default  组件名    默认暴露 
// 
</script>

<style>
/* 组件的样式 */
     
</style>
