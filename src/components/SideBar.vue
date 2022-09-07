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
      {
        id:'5',
        name:'Ayato'
      },
      {
        id:'6',
        name:'Xiangling'
      },
      {
        id:'7',
        name:'Kazuha'
      },
    ]
    }
  },

})
</script>
<style>
*{
  margin:0;
  padding:0;
  box-sizing: border-box;
}
  .sidebar{
    height:100vh;
    width:13vw;
    position: fixed; 
    z-index: 1;
    top: 0; 
    right: 0;
    background-color: #111;
    color:#eee;
    overflow-x: hidden;
    padding: 10px;
  }
  .navigation{
    width:100%;
    height:100%;
    display: block;
    flex-direction: row;
    flex-wrap: wrap;
    overflow-y:scroll;
  }
  .char-nav{
    aspect-ratio: 1/1;
    width:92%;
    height:auto;
    margin:5px;
    background-color: rgba(255, 255, 255, 0.070);
  }

</style>