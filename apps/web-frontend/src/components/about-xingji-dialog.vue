<template>
<v-dialog scrollable max-width='650' v-model="$store.state.showAboutXingjiDialog">
  <v-card v-if="$store.state.showAboutXingjiDialog">
    <v-card-title><div class="text-h5">关于星迹</div></v-card-title>
    <v-card-text style="height: 600px;">
      <h3>丽江星迹旅课文化传播有限公司</h3>
      <p>
        丽江星迹旅课文化传播有限公司是立足云南丽江的天文科普与文化旅游机构，专注于将专业天文观测、自然科学教育与旅游体验相结合。公司依托丽江玉龙雪山的高海拔观星优势，运营金茂璞修雪山天文台、阿美泽天文台等设施，配备国内景区最大口径的半米望远镜及24台全自动望远镜阵列，提供星空观测、深空摄影、科普课程及研学活动服务。其业务覆盖丽江、泸沽湖、香格里拉等多地，致力于天文资源共享与暗夜保护。
      </p>

      <h3>产品与服务</h3>
      <ul class="about-xingji-list">
        <li>星空观测与深空摄影</li>
        <li>天文科普课程</li>
        <li>研学活动服务</li>
      </ul>

      <h3>商务合作</h3>
      <div class="about-xingji-stations">
        <div class="station-item">
          <div class="station-name">甘海子观测站</div>
          <div class="station-desc">与金茂璞修酒店合作</div>
        </div>
        <div class="station-item">
          <div class="station-name">香格里拉观测站</div>
          <div class="station-desc">提供专业全自动天文望远镜设备</div>
        </div>
        <div class="station-item">
          <div class="station-name">宁夏中卫观测站</div>
          <div class="station-desc">与沙漠星星酒店合作</div>
        </div>
        <div class="station-item">
          <div class="station-name">普洱观测站</div>
          <div class="station-desc">与倚象山半山酒店合作</div>
        </div>
      </div>
    </v-card-text>
    <v-card-actions>
      <v-spacer></v-spacer><v-btn text class="blue--text darken-1" @click.native="$store.state.showAboutXingjiDialog = false">关闭</v-btn>
    </v-card-actions>
  </v-card>
</v-dialog>
</template>

<script>
</script>

<style>
.about-xingji-list {
  padding-left: 30px;
  margin-bottom: 16px;
}
.about-xingji-stations {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 16px;
  margin-top: 8px;
}
.station-item {
  padding: 8px 0;
}
.station-name {
  font-weight: bold;
  font-size: 15px;
  margin-bottom: 4px;
}
.station-desc {
  color: #aaa;
  font-size: 13px;
}
</style>
