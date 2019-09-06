<template>
  <div :style="style">
  </div>
</template>

<script>
import { clearInterval } from 'timers';
export default {
  name: 'HelloWorld',
  props: {
    image: String,
    height: Number,
    width: Number,
    loop: Number,
    frame: Number,
    max: Number,
    column: Number,
    row: Number,
  },

  mounted() {
    this.play()
  },

  data(){
    return {
      style: {
        width: this.width + 'px',
        height: this.height + 'px',
        background: `url(${this.image})`,
        backgroundSize: `${this.width * this.column}px ${this.height * this.row}px`,
        backgroundPosition: '0px 0px'
      }
    }
  },
  
  methods: {
    play() {
      let i = 0
      setInterval(() => {
        if(i % this.column) {
          this.$set(this.style, 'backgroundPosition', `${this.width * i}px 0px`)
        } else {
          this.$set(this.style, 'backgroundPosition', `0px ${this.height * i}px`)
        }
        if (i == this.max) {
          i = 0
        }
        i++;
      }, 1000/this.frame);
    }
  }
}
</script>
