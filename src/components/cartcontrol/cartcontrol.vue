<template>
<<<<<<< HEAD
  <div class="cartcontrol">
    <div class="cart-decrease " v-show="food.count>0" @click="decreaseCart">
      <transition name="move">
        <div class="inner icon-remove_circle_outline"></div>
      </transition>
    </div>
    <div class="cart-count" v-show="food.count>0">{{ food.count }}</div>
    <div class="cart-add icon-add_circle" @click="addCart"></div>
=======
  <div class="cartcontral">
    <div class="cart-decrease" v-show="food.count>0"></div>
    <div class="cart-count" v-show="food.count>0">{{ food.count }}</div>
    <div class="cart-add"></div>
>>>>>>> 76e26915bc81d2a549541b816299ce588c036dfe
  </div>
</template>

<script type="text/ecmascript-6">
<<<<<<< HEAD
  import Vue from 'vue'
=======
>>>>>>> 76e26915bc81d2a549541b816299ce588c036dfe
  export default {
    props: {
      food: {
        type: Object
      }
    },
<<<<<<< HEAD
    methods: {
      addCart (event) {
        if (!event._constructed) {
          return
        }
        if (!this.food.count) {
          Vue.set(this.food, 'count', 1)
        } else {
          this.food.count++
        }
      },
      decreaseCart (event) {
        if (!event._constructed) {
          return
        }
        if (this.food.count) {
          this.food.count--
        }
      }
=======
    created () {
      console.log(this.food)
>>>>>>> 76e26915bc81d2a549541b816299ce588c036dfe
    }
  }
</script>

<style lang="stylus" rel="stylesheet/stylus">
<<<<<<< HEAD
  .cartcontrol
    font-size 0
    .cart-decrease
      display inline-block
      padding 6px
      //transition all 0.4s linear
      //.move-enter-active
        //opacity 1
        //transform translate3D(0,0,0)
        //transition: opacity .5s
        .inner
          display inline-block
          line-height 24px
          font-size 24px
          color rgb(0, 160, 220)
        //transition all 0.4s linear
        //transform rotate(0)
      //.move-enter, .move-leave-active
        //opacity 0
        //transform translate3D(24px,0,0)
        //.inner
          //transform rotate(180deg)
    .cart-count
      display inline-block
      vertical-align top
      width 12px
      padding-top 6px
      line-height 24px
      text-align center
      font-size 10px
      color rgb(147, 153, 159)
    .cart-add
      display inline-block
      padding 6px
      line-height 24px
      font-size 24px
      color rgb(0, 160, 220)
=======

>>>>>>> 76e26915bc81d2a549541b816299ce588c036dfe
</style>
