<template>
  <div id="app">
    <!-- <img src="./assets/logo.png"> -->
<!--     <router-view></router-view> -->
    <el-table
      :data="tableData"
      :row-style="headRow"
      border
      highlight-current-row
      @current-change="handleCurrentChange"
      style="width: 100%"
      :default-sort = "{prop: 'date', order: 'descending'}"
      >
      <el-table-column
        type="index"
        width="50">
      </el-table-column>
      <el-table-column
        prop="date"
        label="日期"
        sortable
        width="130">
      </el-table-column>
      <el-table-column
        prop="home"
        label="学校官网"
        width="80">
      </el-table-column>
      <el-table-column
        prop="pudu"
        label="普度教育"
        width="80"
        >
      </el-table-column>
      <el-table-column
        prop="sanhao"
        label="三好教育"
        width="80">
      </el-table-column>
      <el-table-column
        prop="help"
        label="帮助"
        width="55">
      </el-table-column>
      <el-table-column
        prop="production"
        label="产品培训"
        width="80">
      </el-table-column>
      <el-table-column
        prop="guzhang"
        label="故障保修"
        width="80">
      </el-table-column>
      <el-table-column
        prop="yuancheng"
        label="远程协助"
        width="80">
      </el-table-column>
      <el-table-column
        prop="network"
        label="互联"
        width="55">
      </el-table-column>
      <el-table-column
        prop="jiance"
        label="监测"
        width="55">
      </el-table-column>
      <el-table-column
        prop="yingyin"
        label="影音"
        width="55">
      </el-table-column>
      <el-table-column
        prop="option"
        label="设置"
        width="55">
      </el-table-column>
      <el-table-column
        prop="Upan"
        label="U盘"
        width="55">
      </el-table-column>
      <el-table-column
        prop="desktop"
        label="桌面"
        width="55">
      </el-table-column>
      <el-table-column
        prop="close"
        label="关闭"
        width="55">
      </el-table-column>
      <el-table-column
        prop="notice"
        label="通知公告"
        width="80">
      </el-table-column>
      <el-table-column
        prop="yunedu"
        label="云课堂"
        width="68">
      </el-table-column>
      <el-table-column
        prop="memory"
        label="脑王记忆"
        width="80">
      </el-table-column>
      <el-table-column
        prop="jiaohu"
        label="交互"
        width="55">
      </el-table-column>
      <el-table-column
        prop="zhanshi"
        label="展示"
        width="55">
      </el-table-column>
    </el-table>

  </div>
</template>

<script>
export default {
  name: 'app',
  data() {
    return {
      tableData: [{
        date: '2016-05-02',
        home: '0',
        pudu: '2',
        sanhao:'4',
        help:'5',
        production:'3',
        guzhang:'6',
        yuancheng:'7',
        network:'8',
        jiance:'9',
        yingyin:'10',
        option:'12',
        Upan:'13',
        desktop:'14',
        close:'15',
        notice:'1',
        yunedu:'7',
        memory:'9',
        jiaohu:'0',
        zhanshi:'1'
      }, {
        date: '2016-05-04',
        home: '0',
        pudu: '2',
        sanhao:'4',
        help:'5',
        production:'3',
        guzhang:'6',
        yuancheng:'7',
        network:'8',
        jiance:'9',
        yingyin:'10',
        option:'12',
        Upan:'13',
        desktop:'14',
        close:'15',
        notice:'1',
        yunedu:'7',
        memory:'9',
        jiaohu:'0',
        zhanshi:'1'
      }, {
        date: '2016-05-01',
        home: '0',
        pudu: '2',
        sanhao:'4',
        help:'5',
        production:'3',
        guzhang:'6',
        yuancheng:'7',
        network:'8',
        jiance:'9',
        yingyin:'10',
        option:'12',
        Upan:'13',
        desktop:'14',
        close:'15',
        notice:'1',
        yunedu:'7',
        memory:'9',
        jiaohu:'0',
        zhanshi:'1'
      }, {
        date: '2016-05-03',
        home: '0',
        pudu: '2',
        sanhao:'4',
        help:'5',
        production:'3',
        guzhang:'6',
        yuancheng:'7',
        network:'8',
        jiance:'9',
        yingyin:'10',
        option:'12',
        Upan:'13',
        desktop:'14',
        close:'15',
        notice:'1',
        yunedu:'7',
        memory:'9',
        jiaohu:'0',
        zhanshi:'1'
      }]
    }
  },
  methods: {
    formatter(row, column) {
      return row.address;
    },
    handleCurrentChange(val){
       this.currentRow = val;
    },
    headRow(row,index){
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
th:nth-child(2){
   text-align: center;
}
th>div.cell{
  font-size:12px;
   padding-left: 15px!important;
   padding-right: 15px!important;
}
</style>
