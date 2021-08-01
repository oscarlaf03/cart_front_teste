<template>
  <div class="box">
    <div class="order-item__details">
      <p class="is-inline">order id:{{order.id}}</p>
      <ul class='order-item' v-for='item in order.items' :key='item.id'>
        <li>name: {{item.title}} price: {{item.price}} quantity: {{item.quantity}}</li>
      </ul>
    </div>
  </div>

</template>

<script>

export default {
  name: 'OrderListItem',
  props: ['order'],
};
</script>
