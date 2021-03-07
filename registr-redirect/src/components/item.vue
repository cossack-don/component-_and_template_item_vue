<template>
  <div style="background:yellow; margin:10px; padding:15px;">
      <p style="color:green;">paragraph - 1 {{product.title}}</p>
      <p>paragraph - 2 {{product.discr}}</p>
  </div>
</template>

<script>
export default {
// пропсы обычно передаются в дочернем компоненте для принятия их в родительском компоненте


    // передаем пропсы App => item компонент, чтобы отрисовать данные
    // нужно чтобы тип был обьектом,обязательно
    // product это название которые мы баендим в app компоненте, можно назвать произвольно
props: {
    product: {
        type: Object,
        required:true
    }
}
}
</script>
