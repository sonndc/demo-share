<template>
  <div class="first-view">
    <SharedCard title="Thông tin người dùng">
      <template #header-actions>
        <button class="edit-btn">Chỉnh sửa</button>
      </template>
      
      <div class="user-info">
        <p><strong>Họ tên:</strong> Nguyễn Văn A</p>
        <p><strong>Email:</strong> nguyenvana@example.com</p>
        <p><strong>Số điện thoại:</strong> 0123456789</p>
      </div>

      <template #footer>
        <div class="footer-actions">
          <button class="primary-btn">Lưu thay đổi</button>
        </div>
      </template>
    </SharedCard>
  </div>
</template>

<script>
import SharedCard from '@/components/SharedCard.vue'

export default {
  name: 'FirstView',
  components: {
    SharedCard
  }
}
</script>

<style scoped>
.first-view {
  padding: 20px;
}

.edit-btn {
  padding: 6px 12px;
  background-color: #4CAF50;
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

.user-info p {
  margin: 8px 0;
}

.footer-actions {
  display: flex;
  justify-content: flex-end;
}

.primary-btn {
  padding: 8px 16px;
  background-color: #1976D2;
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}
</style> 