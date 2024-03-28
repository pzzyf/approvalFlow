<template>
  <div class="page">
    <Process
      ref="processDesign"
      :conf="mockData.processData"
    />
  </div>
</template>

<script>
// @ is an alias to /src
import Process from "@/components/Process";
import { GET_MOCK_CONF } from "../../api";

export default {
  data() {
    return {
      mockData: null, // 可选择诸如 $route.param，Ajax获取数据等方式自行注入
    };
  },
  mounted() {
    GET_MOCK_CONF().then((data) => {
      
      this.mockData = data
      console.log(this.mockData, '123');
    });
    
  },
  components: {
    Process
  },
};
</script>
<style lang="stylus" scoped>
$header-height = 54px;
.page {
  width: 100vw;
  height: 100vh;
  box-sizing: border-box;
}
</style>
