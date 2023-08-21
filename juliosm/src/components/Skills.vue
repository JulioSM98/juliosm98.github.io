

<template>
    <h2>
        <Typer :text="['Back-End','DevOps','SysAdmin']" pre-type-delay='200' eraseStyle='backspace' type-delay='100' preEraseDelay="800" eraseDelay="100"  caretAnimation='smooth' ></Typer>
    </h2>
</template>

<script lang="ts" >
import {defineComponent} from "vue"
import {Typer} from 'vue3-typer'
import "vue3-typer/dist/vue-typer.css"

export default defineComponent({
    // ...
    components: {
        Typer
    }
})
</script>

<style>
h2{
  text-align: center;
  font-size: 3rem;
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