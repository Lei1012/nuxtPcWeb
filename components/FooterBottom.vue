<template>
  <div class="footer-d-container">
    <div class="footer-d-d">
                <span>枢秘（杭州）信息科技有限公司
                    <a rel="nofollow" href="http://beian.miit.gov.cn/" target="_blank">浙ICP备18019159号-2</a>
                    <a rel="nofollow" href="http://www.beian.gov.cn/portal/registerSystemInfo?recordcode=33010402004047"
                       target="_blank">浙公网安备浙公网安备 33010402004047号</a>
                    举报电话：+8613482207807   举报邮箱：customer@nsnni.com   Copyright © 全民体育</span>
    </div>
  </div>
</template>

<script>

  import { GetCurrentBrowser, GetOs } from '~/utils/systemTool.js'
  import FooterLink from './FooterLink'

  export default {
    name: 'FooterBottom',
    components:{
      FooterLink
    },
    data () {
      return {
        os: '',
        isShowLink:false,
      }
    },
    mounted () {
      this.os = GetOs()
    }
  }
</script>

<style scoped>



  .footer-d-container {
    /*background: #CFD6DE;*/
    height: 50px;
    background: rgba(207, 214, 222, 1);
  }


  .footer-d-d span {
    height: 49px;
    line-height: 49px;
    display: block;
    /*margin-top: 15px;*/
    font-family: PingFangSC-Regular;
    font-size: 14px;
    color: #333333;
  }

  .footer-d-d a {
    font-family: PingFangSC-Regular;
    font-size: 14px;
    color: #333333;
  }


</style>
