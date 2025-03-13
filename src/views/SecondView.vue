<template>
  <div class="second-view">
    <SharedCard title="Thống kê doanh thu">
      <template #header-actions>
        <button class="refresh-btn">Làm mới</button>
      </template>
      
      <div class="statistics">
        <div class="stat-item">
          <h3>Doanh thu tháng</h3>
          <p class="amount">50.000.000 VNĐ</p>
        </div>
        <div class="stat-item">
          <h3>Số đơn hàng</h3>
          <p class="amount">150</p>
        </div>
      </div>

      <template #footer>
        <div class="footer-actions">
          <button class="export-btn">Xuất báo cáo</button>
        </div>
      </template>
    </SharedCard>
  </div>
</template>

<script>
import SharedCard from '@/components/SharedCard.vue'

export default {
  name: 'SecondView',
  components: {
    SharedCard
  }
}
</script>

<style scoped>
.second-view {
  padding: 20px;
}

.refresh-btn {
  padding: 6px 12px;
  background-color: #FF9800;
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

.statistics {
  display: flex;
  gap: 20px;
}

.stat-item {
  flex: 1;
  text-align: center;
  padding: 20px;
  background-color: #f5f5f5;
  border-radius: 8px;
}

.stat-item h3 {
  margin: 0 0 10px 0;
  color: #666;
}

.amount {
  font-size: 1.5rem;
  font-weight: bold;
  color: #2196F3;
  margin: 0;
}

.footer-actions {
  display: flex;
  justify-content: flex-end;
}

.export-btn {
  padding: 8px 16px;
  background-color: #673AB7;
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}
</style> 