<template>
  
</template>

<script>
export default {
  
}
</script>

<style scoped>
    改造计划-整个页面数据驱动的点以及逻辑:
            1.页面重定向获取code

            2.获取code获取用户微信信息(调用微信用户信息保存api)

            3.根据openid已经活动id去访问api,是否具有参与资格api
                3.1 今天已参加活动
                3.2 今天参加活动了,但是奖品未被领取
                3.3 具有参加资格
            
             3.3成立

            4.请求奖品
                4.1 失败
                4.2 成功

             4.2成立

            5.获取奖品名称,根据配置,奖品名称动态修改静态图片资源

            6.核销领奖,调用领取接口api,调用成功,修改stamp的class,并给予提示  


    界面规划-组件化:index.html 入口
            <stamp></stamp> 戳组件
            <received></received> 接收组件       
</style>



