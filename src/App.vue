<template>
  <div class="maintenance-container" role="main" aria-labelledby="main-title">
    <div class="icon-wrapper" aria-hidden="true">
      <svg viewBox="0 0 64 64">
        <circle cx="32" cy="32" r="12" />
        <path d="M32 16 L32 20" stroke-width="2.5" />
        <path d="M32 44 L32 48" stroke-width="2.5" />
        <path d="M44 32 L48 32" stroke-width="2.5" />
        <path d="M16 32 L20 32" stroke-width="2.5" />
        <path d="M40.5 23.5 L43.5 20.5" stroke-width="2.5" />
        <path d="M23.5 40.5 L20.5 43.5" stroke-width="2.5" />
        <path d="M40.5 40.5 L43.5 43.5" stroke-width="2.5" />
        <path d="M23.5 23.5 L20.5 20.5" stroke-width="2.5" />
        <line x1="14" y1="14" x2="22" y2="22" stroke-width="2.8" />
        <line x1="18" y1="10" x2="26" y2="18" stroke-width="2.8" />
        <circle cx="14" cy="14" r="4" stroke-width="1.8" />
      </svg>
    </div>

    <h1 id="main-title" class="title">系统正在维护</h1>

    <p class="description">
      为了给您提供更稳定的服务，我们正在进行例行升级。<br />
      稍后将恢复访问，感谢您的耐心等待。
    </p>
  </div>
</template>

<script setup>
</script>

<style scoped>
.maintenance-container {
  text-align: center;
  max-width: 480px;
  margin: 0 auto;
}

.icon-wrapper {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 96px;
  height: 96px;
  background: #f5f7fa;
  border-radius: 50%;
  margin-bottom: 28px;
}

.icon-wrapper svg {
  width: 48px;
  height: 48px;
  stroke: #2c3e50;
  stroke-width: 1.8;
  fill: none;
  stroke-linecap: round;
  stroke-linejoin: round;
}

.title {
  font-size: 30px;
  font-weight: 600;
  color: #1e293b;
  letter-spacing: -0.3px;
  margin-bottom: 12px;
}

.description {
  font-size: 16px;
  line-height: 1.7;
  color: #64748b;
  margin: 0 auto;
}

@media (max-width: 480px) {
  .icon-wrapper {
    width: 76px;
    height: 76px;
  }

  .icon-wrapper svg {
    width: 38px;
    height: 38px;
  }

  .title {
    font-size: 24px;
  }

  .description {
    font-size: 15px;
  }
}
</style>
