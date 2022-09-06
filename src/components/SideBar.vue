<template>
  <div class="sidebar" >
    <div class="navigation">
      <div class="char-nav" v-for="char in characters" v-bind:key="char.id">{{char.name}}</div>
    </div>
  </div>
</template>

<script>


export default({
  name:"SideBar",
  data() {
    return{
      
      
      characters:[
      {
        id:'1',
        name:'Tighnari'
      },
      {
        id:'2',
        name:'Kujou Sarah'
      },
      {
        id:'3',
        name:'Kuki Shinobu'
      },
      {
        id:'4',
        name:'Collei'
      },
    ]
    }
  },

})
</script>
