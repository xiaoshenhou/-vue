<template>
  <div>
            <hr>
            <h2 :style="{fontFamily:ziTi}">学生信息:</h2>
            <h2>学生姓名：{{name}}</h2>
            <h2>学生年龄：{{age}}</h2>
            <h2>学生喜欢的女孩：
                <ul>
                    <li v-for="(I) in myLover" :key="I.id">
                        {{I.name}} -- {{I.age}}
                    </li>
                </ul>
            </h2>
        </div>
</template>

<script>
    export default {
              data(){
                return {
                    ziTi:"黑体",
                    name: "李培松",
                    age:18,
                    myLover:[
                        {id:001,name:"高瑞丽",age:21},
                        {id:002,name:"郭瑞瑾",age:21},
                        {id:003,name:"李盼盼",age:21},
                        {id:004,name:"李明",age:24},
                    ]
                }
            }
    }
</script>

<style>

</style>