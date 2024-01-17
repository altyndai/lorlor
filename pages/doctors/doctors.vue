<template>
  <div class="container">
    <div class="grid">
      <div class="col-12 md:col-4 lg:col-4 mb-5" >
        <div class="card-check" style="background:#FFFFFF; padding: 45px 30px">
          <div class="card">
            <div class="flex flex-column gap-3 mb-6">
              <h3>Филиал</h3>
              <div v-for="category in radio" :key="category.key" class="flex align-items-center">
                <RadioButton v-model="selectedCategory" :inputId="category.key" name="pizza" :value="category.name" />
                <label :for="category.key" class="ml-3">{{ category.name }}</label>
              </div>
            </div>
          </div>
          <div class="card">
            <div class="flex flex-column gap-3 mb-6">
              <h3>Направление врача</h3>
              <div v-for="category of categories" :key="category.key" class="flex align-items-center">
                <Checkbox v-model="selectedCategories" :inputId="category.key" name="category" :value="category.name" />
                <label :for="category.key" class="ml-3">{{ category.name }}</label>
              </div>
            </div>
          </div>
          <div class="card">
            <div class="flex flex-column gap-3">
              <h3>Стиль работы</h3>
              <div v-for="category of categorie" :key="category.key" class="flex align-items-center">
                <Checkbox v-model="selectedCategorie" :inputId="category.key" name="category" :value="category.name" />
                <label :for="category.key" class="ml-3">{{ category.name }}</label>
              </div>
            </div>
          </div>
          <button class="button font" style="padding:10px 50px; margin-left: -1px; margin-top: 30px">
            Сбросить
          </button>
        </div>
      </div>
      <div class="col-12 md:col-8 lg:col-8 mb-5">
        <section class="pt-20">
              <div v-for="el in cards" :key="el.id" class="mb-6 pl-6 ">
                <div class=" card flex-column sm:flex-row flex p-4 bg-white w-full h-full">
                  <div class="card-animation-left" />
                  <div class="">
                    <img class="card-img" :src="el.img" alt="">
                  </div>
                  <div class="ml-4 mt-5 ">
                    <h1 class="card-name">
                      <router-link to="">
                        {{ el.name }}
                      </router-link>
                    </h1>
                    <div class="card-job-title">
                      <span>{{ el.expert }}</span>
                    </div>
                    <p class="main-description mt-4">
                      {{ el.profession }}
                    </p>
                    <div class="main-description main-description--bg-hover">
                      <p>
                        стаж: <b>{{ el.experience }}</b>
                      </p>
                      <div class="rectangle" />
                    </div>
                    <div class="card-animation-right" />
                  </div>
                </div>
              </div>
        </section>
      </div>
    </div>
  </div>
</template>

<script setup>
const cards = ref([
  {
    id: 1,
    img: '/img/photo_5341629398899609206_x.jpg',
    name: 'Галкин Алексей Владимирович',
    expert: 'эксперт по лор-патологиям',
    profession: 'оториноларинголог, ринохирург',
    experience: '16 лет'
  },
  {
    id: 2,
    img: '/img/photo_5341629398899609207_x.jpg',
    name: 'Садыхов Рагим Агаларович',
    expert: 'эксперт по лор-патологиям',
    profession: 'оториноларинголог, ринохирург',
    experience: '8 лет'
  },
  {
    id: 3,
    img: '/img/photo_5341629398899609208_x.jpg',
    name: 'Чуприков Роман Сергеевич',
    expert: 'эксперт по лор-патологиям',
    profession: 'оториноларинголог, ринохирург, фониатр, врач высшей категории',
    experience: '21 лет'
  },
  {
    id: 4,
    img: '/img/photo_5341629398899609209_x.jpg',
    name: 'Оганесян Тигран Сергеевич',
    expert: 'заведующий отделением, экс',
    profession: 'оториноларинголог, ринохирург',
    experience: '20 лет'
  },
  {
    id: 5,
    img: '/img/photo_5341629398899609210_x.jpg',
    name: 'Якушев Анатолий Андреевич',
    expert: 'ведущий врач клиники',
    profession: 'оториноларинголог, отохирург',
    experience: '13 лет'
  },
  {
    id: 6,
    img: '/img/photo_5341629398899609211_x.jpg',
    name: 'Соколова Алла Васильевна',
    expert: 'кандидат медицинских наук',
    profession: 'оториноларинголог, отохирург, врач высшей категории',
    experience: 'свыше 35 лет'
  },
  {
    id: 7,
    img: '/img/photo_5341629398899609212_x.jpg',
    name: 'Старосветский Андрей Борисович',
    expert: 'кандидат медицинских наук',
    profession: 'оториноларинголог, ринохирург',
    experience: '22 лет'
  },
  {
    id: 8,
    img: '/img/photo_5341629398899609213_x.jpg',
    name: 'Мосейкина Лилия Алексеевна',
    expert: 'кандидат медицинских наук',
    profession: 'отохирург',
    experience: '31 лет'
  },
  {
    id: 9,
    img: '/img/photo_5341629398899609213_x.jpg',
    name: 'Гилилов Вадим Изроевич',
    expert: 'эксперт по лор-патологиям',
    profession: 'оториноларинголог, ринохирург',
    experience: '13 лет'
  }
])
const selectedCategory = ref('Production')
const radio = ref([
  { name: 'Все филиалы', key: 'B' },
  { name: 'Цветной бульвар', key: 'S' },
  { name: 'Преображенская площадь', key: 'P' },
  { name: 'Бульвар Дмитрия Донского', key: 'D' },
  { name: 'Мичуринский проспект', key: 'M' },
  { name: 'Фили', key: 'F' }
])
const categories = ref([
  {
    name: 'Аллерголог-иммунолог',
    key: '1'
  },
  {
    name: 'Врач УЗИ',
    key: '2'
  },
  {
    name: 'Выезд на дом',
    key: '3'
  },
  {
    name: 'Кардиолог',
    key: '4'
  },
  {
    name: 'Массажист',
    key: '5'
  },
  {
    name: 'Медсестра',
    key: '6'
  },
  {
    name: 'Невролог',
    key: '7'
  },
  {
    name: 'Отоларинголог',
    key: '8'
  },
  {
    name: 'Отоневролог',
    key: '9'
  },
  {
    name: 'Отохирург',
    key: '10'
  },
  {
    name: 'Психолог',
    key: '11'
  },
  {
    name: 'Пульмонолог',
    key: '12'
  },
  {
    name: 'Рефлексотерапевт',
    key: '13'
  },
  {
    name: 'Ринохирург',
    key: '14'
  },
  {
    name: 'Сурдолог',
    key: '15'
  },
  {
    name: 'Терапевт',
    key: '16'
  },
  {
    name: 'Флеболог',
    key: '17'
  },
  {
    name: 'Фониатр',
    key: '18'
  },
  {
    name: 'Эндокринолог',
    key: '19'
  }
])
const selectedCategories = ref([''])
const categorie = ref([
  {
    name: 'Cтрогий доктор',
    key: '1'
  },
  {
    name: 'Доктор, с которым можно поговорить как с партнёром',
    key: '2'
  },
  {
    name: 'Понимающий и эмоциональный доктор',
    key: '3'
  }
])
const selectedCategorie = ref(['Marketing'])
</script>
