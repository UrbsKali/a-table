<template>
  <div class="card">
      <div class="card_header">
        <i
        class="bx"
        :class="icon || 'bx-square-rounded'"
        /> 
          <span class="title">{{ title }}</span>

          
      </div>
      <div class="card_content">

      </div>
  </div>
</template>

<script>
export default {
  props: {
    icon: {
      type: String,
      default: '',
    },
    title: {
      type: String,
      default: 'Oyé',
    },
    description: {
      type: String,
      default: 'Oya',
    }
  },
}
</script>

<style scoped>
.icon {
  display: flex;
}
.title{
    padding: 5px 5px 5px 20px;
    font-size: 30px;
    font-weight: 800;
}
.card {
  background-color: #11101d;
  color: #fff;
  border-radius: 16px;
  padding: 24px;
  width: 327px;
  font-size: 1.5rem;
  box-shadow: 0 25px 50px 0 rgba(0,0,0,0.1);
  
}
@media screen and (min-width: 768px) {
    .card {
        font-size: 1.6rem;
        width: 350px;
        padding-bottom: 32px;
    }
}

.card_content {
    display: flex;
    flex-direction: column;
    gap: 12px;
    padding: 24px 0 16px 0;
}
@media screen and (min-width: 768px) {
    .card_content {
        gap: 16px;
        padding: 24px 0;
    }
}
.card_name {
    color: white;
    font-size: 2.2rem;
    font-weight: bold;
    cursor: pointer;
    
}
.card_name:hover {
    color: #00FFF8;
}
.card_description {
    font-size: 1.8rem;
    line-height: 2.6rem;
    font-weight: lighter;
}

  

.fade-enter-active,
.fade-leave-active {
    transition: 0.25s ease-out;
}
.fade-leave-to,
.fade-enter-from {
  opacity: 0;
}
</style>