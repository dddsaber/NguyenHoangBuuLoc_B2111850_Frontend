<script>
export default {
  props: {
    contact: { type: Object, required: true },
  },
};
</script>

<template>
  <div>
    <div class="p-1"><strong>Tên:</strong>{{ contact.name }}</div>
    <div class="p-1"><strong>E-mail:</strong>{{ contact.email }}</div>
    <div class="p-1"><strong>Địa chỉ:</strong>{{ contact.address }}</div>
    <div class="p-1"><strong>Điện thoại:</strong>{{ contact.phone }}</div>
    <div class="p-1">
      <strong>Liên hệ yêu thích:&nbsp;</strong>
      <i class="fas fa-check" v-if="contact.favourite"></i>
      <i class="fas fa-times" v-else></i>
    </div>
  </div>
</template>
