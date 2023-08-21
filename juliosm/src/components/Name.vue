

<template>
    <h1>
        <Typer text='Julio Sejas' repeat="0" pre-type-delay='100' type-delay='100' caretAnimation='smooth' ></Typer>
    </h1>
</template>

<script lang="ts" >

import {defineComponent} from "vue"
import {Typer} from "vue3-typer"
import "vue3-typer/dist/vue-typer.css"

export default defineComponent({

    components: {
        Typer
    }
})
</script>

<style>
h1{
  text-align: center;
  font-size: 4rem;
  .vue-typer {    
    --char-typed-color: #4E9A06;
    --caret-idle-color: #4E9A06;
    --caret-typing-color: #4E9A06;
    --caret-complete-color: #4E9A06;
    
    .caret {
      &.complete {
        display: inline-block;
      }

    }
  }
}

</style>