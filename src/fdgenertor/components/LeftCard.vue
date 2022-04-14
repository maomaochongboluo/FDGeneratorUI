<template>
  <div>
    <el-row>
      <el-col :span="12">
        <div class="left-card">
          <el-button type="primary" round @click="say(testData)">生成数据</el-button>
        </div>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: "LeftCard",
  data: function () {
    return {
      testData: 1,
    };
  },
  methods: {
    say: function (message) {
      this.testData = message + 1;
      alert(this.testData);
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.left-card {
  height: 800px;
  background: white;
  margin: 100px;
  padding: 30px;
  box-shadow: 15px 16px 20px 0px rgba(44, 50, 50, 0.68);
  border-radius: 5px;
}
</style>
