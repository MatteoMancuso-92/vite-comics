<script>
export default {
    data () {
    
    return {
        navbaritems:[
            
            {
                name: "CHARACTERS",
                src: "#",
                active: false,
            },
            {
                name: "COMICS",
                src: "#",
                active: false,
            },
            {
                name: "MOVIES",
                src: "#",
                active: false,
            },
            {
                name: "TV",
                src: "#",
                active: false,
            },
            {
                name: "GAMES",
                src: "#",
                active: false,
            },
            {
                name: "COLLECTIBLES",
                src: "#",
                active: false,
            },
            {
                name: "VIDEOS",
                src: "#",
                active: false,
            },
            {
                name: "FANS",
                src: "#",
                active: false,
            },
            {
                name: "NEWS",
                src: "#",
                active: false,
            },
            {
                name: "SHOP",
                src: "#",
                active: false,
            },
        ]
    }
}
}
</script>



<template>
  <nav>
      <ul>
        <li v-for="menuItem in navbaritems" :key="menuItem.name">
				<a :href="menuItem.src">{{ menuItem.name }}</a>
		</li>
      </ul>
    </nav>
</template>



<style lang="scss" scoped>
@use './../assets/styles/partials/variables' as *;
nav{
    height: 100%;
    @include align-center;
  }
  
ul{
    @include align-center;
    gap: 1em;
    list-style: none;
    height: 100%;
  }

  
  li{
    @include align-center;
    height: 100%;
    padding: .5em;
    font-size: 14px;
    &:hover{
      border-bottom: 3px solid $brand-color;
      cursor: pointer;
    }
    &:active{
      background-color: lightgray;
    }

    
    a{
    text-decoration: none;
    color: black;
    }
  }
  
  
</style>