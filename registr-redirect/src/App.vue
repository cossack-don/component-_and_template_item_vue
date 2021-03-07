<template>
  <div id="app">
<!-- Компонент переиспользуемый ITEM -->

<!-- баендим данные :product = item . Получаем данные в данном компоненте APP => array with obj 
чтобы отрисовать все данные из обьекта который получили циклом for , мы задаем product = item

 -->
    <imp v-for="(item,index) in items" :key="index"
    :product="item"
    />
<!-- END Компонент переиспользуемый ITEM -->
  </div>
</template>



<script>
import imp from '@/components/item'

export default {
components:{
  imp
},
data() {
  return {
    // array data
    items:[
      {
        title:'title-1',
        discr:'discr------2'
      },
            {
        title:'title-2',
        discr:'discr------233'
      },
            {
        title:'title-3',
        discr:'discr------2333'
      }
    ]
  }
},

}
</script>
