<template>
  <div class="shared-card">
    <div>Warning screen 1</div>
    <div class="card-header">
      <h2>{{ title }}</h2>
      <slot name="header-actions"></slot>
    </div>
    <div class="card-content">
      <slot></slot>
    </div>
    <div class="card-footer" v-if="$slots.footer">
      <slot name="footer"></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SharedCard',
  props: {
    title: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>
.shared-card {
  border: 1px solid #ddd;
  border-radius: 8px;
  padding: 16px;
  margin: 16px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.card-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 16px;
}

.card-header h2 {
  margin: 0;
  font-size: 1.5rem;
}

.card-content {
  margin-bottom: 16px;
}

.card-footer {
  border-top: 1px solid #eee;
  padding-top: 16px;
}
</style> 