<template>
  <div class="book_area">
    <p>perry</p>
    <img class="img" :src="require('@/assets/BOOK.png')" :alt="imageDescription">
    <el-button class="ddd">默认按钮</el-button>
    <el-input v-model="input" placeholder="请输入内容"></el-input>
    <el-table
      :data="tableData"
      style="width: 50%"
      class="yyy">
      <el-table-column
        prop="date"
        label="日期"
        width="180">
      </el-table-column>
      <el-table-column
        prop="name"
        label="姓名"
        width="180">
      </el-table-column>
      <el-table-column
        prop="address"
        label="地址">
      </el-table-column>
    </el-table>
  </div>
</template>
  
<script>
  export default {
    name: 'book',
    data() {
      return {
        imageDescription: 'Description of the image',
        input: '',
        tableData: [{
            date: '2016-05-02',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1518 弄'
          }, {
            date: '2016-05-04',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1517 弄'
          }, {
            date: '2016-05-01',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1519 弄'
          }, {
            date: '2016-05-03',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1516 弄'
          }]
      };
    }
  };
</script>
<style>
.book_area{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  color: yellow;
}
    .ddd{
      text-align: center;
    }
    .img{
        width: 200px;
        height: 200px;
    }
    .yyy{
      color: red;
    }
</style>
  
  
