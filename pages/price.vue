<template>
  <div>
    <hr>
    <div class="container">
      <div>
        <Breadcrumb class="p-component--crumbing ml--4" :home="home" :model="items" />
      </div>
      <p class="lor__txt mt-6">Цены носят ознакомительный характер и не являются публичной офертой.</p>
      <h1 class="title mt--12 mb-6">Прайс-лист на ЛОР услуги</h1>
      <span class="p-input-icon-right mb-6">
            <i class="pi pi-search"  />
            <InputText v-model="value1" style="width: 162.5vh; border-radius: 4px; padding: 15px"/>
            </span>
      <div class="flex justify-content-between w-full mb-3">
        <p class="text-base md:text-xl font-semibold mb-0">Услуга</p>
        <div class="flex align-items-center cursor-pointer" >
          <img class="accordion-img--all w-0.7rem opacity-80 mr-2" src="https://www.svgrepo.com/show/108052/arrow-down-filled-triangle.svg" alt="">
          <h4 class="text-base md:text-xl font-semibold my-0">Цена</h4>
        </div>
      </div>
      <Accordion :multiple="true" :activeIndex="[0]">
        <AccordionTab>
          <template #header>
            <div class="flex justify-content-between w-full">
              <p class="text-base md:text-xl font-semibold mb-0">Консультация лора</p>
              <img class="accordion-img w-0.7rem opacity-80" src="https://www.svgrepo.com/show/108052/arrow-down-filled-triangle.svg" alt="">
            </div>
          </template>
          <template #default>
            <div v-for="price in prices">
              <div class="flex align-items-center justify-content-between w-full p-4 hover:bg-[#dee2e6]">
                <p class="text-base md:text-xl font-light mb-0">{{price.caption}}</p>
                <p class="text-base md:text-xl">{{price.number}}</p>
              </div>
            </div>
          </template>
        </AccordionTab>
        <AccordionTab>
          <template #header>
            <div class="flex justify-content-between w-full ">
              <p class="text-base md:text-xl font-semibold mb-0">Консультация лора</p>
              <img class="accordion-img w-0.7rem opacity-80" src="https://www.svgrepo.com/show/108052/arrow-down-filled-triangle.svg" alt="">
            </div>
          </template>
          <template #default>
            <div v-for="price in prices">
              <div class="flex align-items-center justify-content-between w-full p-4 hover:bg-[#dee2e6]">
                <p class="text-base md:text-xl font-light mb-0">{{price.caption}}</p>
                <p class="text-base md:text-xl">{{price.number}}</p>
              </div>
            </div>
          </template>
        </AccordionTab>
        <AccordionTab>
          <template #header>
            <div class="flex justify-content-between w-full ">
              <p class="text-base md:text-xl font-semibold mb-0">Консультация лора</p>
              <img class="accordion-img w-0.7rem opacity-80" src="https://www.svgrepo.com/show/108052/arrow-down-filled-triangle.svg" alt="">
            </div>
          </template>
          <template #default>
            <div v-for="price in prices">
              <div class="flex align-items-center justify-content-between w-full p-4 hover:bg-[#dee2e6]">
                <p class="text-base md:text-xl font-light mb-0">{{price.caption}}</p>
                <p class="text-base md:text-xl">{{price.number}}</p>
              </div>
            </div>
          </template>
        </AccordionTab>
      </Accordion>
      <p class="lor__txt mt-8">Своевременное обращение к врачу поможет сохранить Ваше здоровье.
        Не откладывайте лечение, звоните прямо сейчас. Мы работаем круглосуточно в Москве.</p>
      <p class="lor-info__subtitle pb-6">
        тел.: <a class="tel" href="#"> 8 (495) 266-28-73 </a> (круглосуточно)
      </p>
    </div>
  </div>
</template>

<script setup lang="ts">
const value1 = ref(null)
const prices = ref([
  {
    caption: 'Консультация заведующего лор-отделением, первичная',
    number: '7,000 P'
  },
  {
    caption: 'Консультация заведующего лор-отделением, повторная',
    number: '4,900 P'
  },
  {
    caption: 'Консультация лор-эксперта с эндоскопией, первичная  ',
    number: '5,000 P'
  },
  {
    caption: 'Консультация лор-эксперта, повторная  ',
    number: '3,500 P'
  },
  {
    caption: 'Консультация отоларинголога-сурдолога с эндоскопией, первичная  ',
    number: '6,500 P'
  },
  {
    caption: 'Консультация отоларинголога-сурдолога, повторная  ',
    number: '4,000 P'
  },
  {
    caption: 'Консультация ведущего врача-отоларинголога с эндоскопией, первичная  ',
    number: '3,900 P'
  },
  {
    caption: 'Консультация ведущего врача-отоларинголога с эндоскопией, повторная',
    number: '2,900 P'
  },
  {
    caption: 'Консультация врача-отоларинголога с эндоскопией, первичная',
    number: '3,300 P'
  },
  {
    caption: 'Консультация врача-отоларинголога с эндоскопией, повторная',
    number: '2,000 P'
  },
  {
    caption: 'Консультация отохирурга, КМН, первичная  ',
    number: '5,000 P'
  },
  {
    caption: 'Консультация отохирурга, КМН, повторная  ',
    number: '3,500 P'
  },
  {
    caption: 'Второе мнение Консилиум врачей',
    number: '7,700 P'
  }
])
const home = ref({
  label: 'Главная',
  to: '/'
})
const items = ref([
  { label: 'Цены' }
])

</script>

<style scoped>

</style>
