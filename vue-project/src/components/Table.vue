<template>
  <el-table :data="tableData" border style="width: 80vw">
    <el-table-column prop="fileName" label="文档名称" width="300" />
    <el-table-column prop="file" label="文件">
      <template slot="“scope”">
        <el-image style="width: 100px; height: 100px" :src="scope.row.file" />
      </template>
    </el-table-column>
    <el-table-column prop="score" label="分值" />
    <el-table-column prop="name" label="姓名" />
  </el-table>
</template>

<script lang="ts" setup>
const tableData = [
  {
    fileName: '文件1',
    file: 'https://avatars.githubusercontent.com/u/31693925?v=4',
    score: '99',
    name: '小明'
  },
  {
    fileName: '文件2',
    file: 'https://avatars.githubusercontent.com/u/31693925?v=4',
    score: '94',
    name: '小兰'
  },
  {
    fileName: '文件3',
    file: 'https://avatars.githubusercontent.com/u/31693925?v=4',
    score: '89',
    name: '小杨'
  },
  {
    fileName: '文件4',
    file: 'https://avatars.githubusercontent.com/u/31693925?v=4',
    score: '200',
    name: '小马'
  }
]
</script>
