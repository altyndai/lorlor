<script setup lang="ts">
definePageMeta({
  layout: 'children'
})
const product = ref([
  {
    title: 'Большая забота',
    subtitle: 'о маленьких пациентах',
    link: 'Узнайне подробнее >>',
    image: 'https://lorlor.ru/content/images/slider/slider2-2/bg.jpg'
  },
  {
    title: 'Бережем главное',
    subtitle: 'у деток все пройдет',
    link: 'Узнайне подробнее >>',
    image: 'https://lorlor.ru/content/images/slider/slider2-1/bg.jpg'
  }, {
    title: 'Большая забота',
    subtitle: 'о маленьких пациентах',
    link: 'Узнайне подробнее >>',
    image: 'https://lorlor.ru/content/images/slider/slider2-2/bg.jpg'
  }, {
    title: 'Бережем главное',
    subtitle: 'у деток все пройдет',
    link: 'Узнайне подробнее >>',
    image: 'https://lorlor.ru/content/images/slider/slider2-1/bg.jpg'
  }
])
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
  }
])
</script>
<template>
  <div>
  <section class="products mb-8">
    <Carousel
        :value="product"
        :num-visible="1"
        :num-scroll="1"
        circular
        :autoplay-interval="4000"
    >
      <template #item="slotProps">
        <div class="grid">
          <div class="col-12 md:col-6">
            <div class="relative p-5 sm:p-7 md:p-8 h-full flex flex-column justify-content-center">
              <img src="/public/img/border-left.svg.svg" class="animation-icon--left w-3rem sm:w-1 absolute top-0 left-0 " alt="">
              <h4 class="mb-1 text-5xl md:text-7xl text-blue-700 w-6">
                {{ slotProps.data.title }}
              </h4>
              <h6 class="text-left mt-0 text-4xl text-red-400">
                ${{ slotProps.data.subtitle }}
              </h6>
              <a v-if="slotProps.data.link" :href="slotProps.data.link" />
              <img src="/public/img/border-right.svg.svg" class="animation-icon--right w-3rem sm:w-1 absolute bottom-0 right-0" alt="">
            </div>
          </div>
          <div class="col-12 md:col-6">
            <img :src="slotProps.data.image" class="w-full h-15rem md:h-30rem object-cover" style="object-position: center" alt="">
          </div>
        </div>
      </template>
    </Carousel>
  </section>
    <section>
      <div class="equipment marker">
        <div class="container">
          <h1 class="title">
            Детский ЛОР в Москве
          </h1>
          <p class="lor__txt">
            Профилактика и лечение лор-заболеваний у детей является одним из основных профилей деятельности нашей клиники. Клиника приспособлена для приема самых маленьких пациентов, современное медицинское оборудование оснащено специальными средствами для оказания медицинской помощи детям (специальное лор-оборудование, адаптированное для работы с детьми). В нашей клинике детский лор-врач работает круглосуточно.
          </p>
          <img class="equipment__img" src="https://lorlor.ru/content/images/children/lorlor_devochka_malish.jpg" alt="fffffffff">
          <h1 class="title pb-4">
            Опытные детские лор-врачи
          </h1>
          <p class="lor__txt">
            Врачи клиники имеют огромный опыт лечения детей всех возрастных категорий, обладают специальными навыками общения с детьми и способны оказать своевременную и высококвалифицированную медицинскую помощь, учитывая возрастные особенности диагностики и лечения ребенка. К каждому маленькому пациенту применяется индивидуальный подход.
          </p>
          <img class="equipment__img" src="https://lorlor.ru/content/images/children/lorlor_listova_rebenok.jpg" alt="fffffffff">
          <p class="lor__txt">На фото ведущий врач клиники проводит первичный осмотр ребенка.</p>
          <h1 class="title pb-4">
            Детский лор-врач круглосуточно
          </h1>
          <p class="lor__txt">
            Прием детей в нашей клинике осуществляется в круглосуточном режиме. Если Ваш ребенок испытывает резкие боли в ухе или горле в вечернее или ночное время, обязательно обратитесь к детскому лор-врачу незамедлительно, так как нет никакой необходимости ждать приема врача до утра.
          </p>
          <img class="equipment__img" src="https://lorlor.ru/content/images/children/lorlor_malish.jpg" alt="fffffffff">
          <h1 class="title pb-4">
            Детский лор на дом
          </h1>
          <p class="lor__txt">
            Для удобства наших пациентов в клинике организована служба вызова детского лор-врача на дом. В случае если у Вашего ребенка температура или Вы по объективным причинам не можете самостоятельно посетить клинику, свяжитесь с администратором клиники и вызовите детского лор-врача на дом. Прием заявок осуществляется круглосуточно.
          </p>
          <h1 class="title pb-4">
            Современное оборудование
          </h1>
          <p class="lor__txt">
            При работе с детьми врачи клиники используют самое современное оборудование:
          </p>
          <ul>
            <li class="li">
              эндоскопическое исследование лор-органов с возможностью визуализации изображения на экран компьютера
            </li>
            <li class="li">
             осмотр лор-органов с помощью микроскопа
            </li>
            <li class="li">
             тимпанометр
            </li>
            <li class="li">
             аудиометр
            </li>
            <li class="li">
              лор-комбайн
            </li>
            <li class="li">
             физиотерапевтический аппарат Милта
            </li>
          </ul>
          <h1 class="title pb-4">
            Качественная диагностика
          </h1>
          <p class="lor__txt">
            Используя технические возможности оборудования и передовые методики, детский лор-врач сможет уже на первом приеме поставить диагноз, провести необходимые дополнительные лабораторные и инструментальные исследования и назначить правильное лечение вашему малышу. Клиника предоставляет свои услуги семь дней в неделю в круглосуточном режиме, поэтому ваш малыш ни на секунду не останется без профессиональной заботы и внимания наших врачей.
          </p>
          <img class="equipment__img" src="https://lorlor.ru/content/images/diagnostics/lorlor_endoskopiya.jpg" alt="fffffffff">
          <p class="lor__txt">На фото ведущий врач клиники проводит первичный осмотр ребенка с помощью видеоэндоскопа.</p>
          <h1 class="title pb-4">
            Передовые методики лечения
          </h1>
          <p class="lor__txt">
            Врачи занимаются лечением и профилактикой рецидивов следующих заболеваний:
          </p>
          <ul>
            <li class="li">
              аденоидит,
            </li>
            <li class="li">
              гипертрофия аденоидов,
            </li>
            <li class="li">
              хронический тонзиллит,
            </li>
            <li class="li">
              ангина,
            </li>
            <li class="li">
              ОРВИ,
            </li>
            <li class="li">
              частые простудные заболевания,
            </li>
            <li class="li">
              средний отит,
            </li>
            <li class="li">
              наружный отит,
            </li>
            <li class="li">
              нейросенсорная тугоухость,
            </li>
            <li class="li">
              ларингит,
            </li>
            <li class="li">
              трахеит,
            </li>
            <li class="li">
              бронхит и др.
            </li>
          </ul>
          <p class="lor__txt">
            Применяются следующие консервативные методы лечения:
          </p>
          <ul>
            <li class="li">
              промывание носа методом перемещения,
            </li>
            <li class="li">
              промывание лакун небных миндалин,
            </li>
            <li class="li">
              продувание ушей по Политцеру,
            </li>
            <li class="li">
              катетеризация слуховой трубы с ведением лекарственных веществ,
            </li>
            <li class="li">
              пневмомассаж барабанных перепонок и др.
            </li>
          </ul>
          <p class="lor__txt">
            Медикаментозное лечение дополняется физиотерапевтическими процедурами с помощью аппарата МИЛТА, галотерапии (соляная комната). В соляной комнате дети не будут скучать и найдут чем заняться - посмотреть мультфильмы, рисовать картины или же почитать книжки с родителями.
          </p>
          <img class="equipment__img" src="https://lorlor.ru/content/images/fizio/lorlor_fizio.jpg" alt="fffffffff">
          <p class="lor__txt">На фото медсестра Клиники уха, горла и носа проводит физиотерапевтическую процедуру с помощью аппарата Милта.</p>
          <p class="lor__txt">При назначении лабораторных исследований, требующих забора крови, медсестры безболезненно и без дополнительной психологической нагрузки выполнят эту работу.</p>
          <h1 class="title pb-4">
            Оперативное лечение
          </h1>
          <p class="lor__txt">
            При необходимости в клинике проводится оперативное лечение: тонзиллотомия (частичное удаление небных миндалин при хроническом тонзиллите) с помощью радиоволнового аппарата Сургитрон, тонзиллэктомия (полное удаление небных миндалин при хроническом тонзиллите), аденотомия при гипертрофии аденоидов под контролем эндоскопа, шунтирование барабанной перепонки при стойком экссудативном среднем отите.
          </p>
          <img class="equipment__img" src="https://lorlor.ru/content/images/surgery/adenoidy.jpg" alt="fffffffff">
          <p class="lor__txt">На фото эксперт по лор-патологиям <a class="a" href="#">Оганесян Тигран Сергеевич</a> проводит операцию по
            <a class="a" href="#">удалению аденоидов у ребенка</a> под общим наркозом комбинированным методом..</p>
          <h1 class="title pb-4">
            Анестезия
          </h1>
          <p class="lor__txt">
            Оперативное лечение, такое как тонзиллэктомия, аденотомия, проходит под общим обезболиванием (наркозом) с помощью современных безопасных препаратов, применяемых в течение многих лет в детской практике.
          </p>
          <p class="lor__txt">
            Детские анестезиологи, имеющие многолетний опыт работы с детьми на базе Детской клинической больницы им. Н.Ф. Филатова, сделают оперативное лечение вашего ребенка безболезненным и безопасным.
          </p>
          <p class="lor__txt">
            Бригада детских хирургов под контролем видеоэндоскопии, применяя радиоволновой аппарат Сургитрон для уменьшения кровоточивости тканей, проведет необходимый объем оперативного лечения.
          </p>
          <h1 class="title pb-4">
            Послеоперационный период
          </h1>
          <p class="lor__txt">
            Послеоперационный период ребенок проведет в комфортной палате, в которой родители имеют возможность разместиться вместе с малышом. Клиника работает круглосуточно, ребенок будет всегда под надзором дежурного врача.
          </p>
          <p class="lor__txt">
            Доверяйте здоровье своих детей профессионалам, чтобы их жизнь была долгой и счастливой без хронических заболеваний.
          </p>
          <h1 class="title pb-4">
            Видео
          </h1>
          <img class="equipment__img" src="../public/img/video.png" alt="fffffffff">
          <p class="lor__txt"></p>
          <p class="lor__txt">Своевременное обращение к врачу поможет сохранить Ваше здоровье.
            Не откладывайте лечение, звоните прямо сейчас. Мы работаем круглосуточно в Москве.</p>
          <p class="lor-info__subtitle pb-6">
            тел.: <a class="tel" href="#"> 8 (495) 266-28-73 </a> (круглосуточно)
          </p>
      </div>
      </div>
    </section>
    <div style="background: #f2f2f2">
      <section class="bg-gray-100 pt-20">
        <div class="container">
          <h1 class="main-title main-title--card mb-6">
            Лор-врачи, осуществляющие прием детей
          </h1>
          <div class="grid -ml-6">
            <div v-for="el in cards" :key="el.id" class="col-12 xl:col-6 mb-6 pl-6 ">
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
          </div>
          <p class="lor__txt"></p>
          <p class="lor__txt">Своевременное обращение к врачу поможет сохранить Ваше здоровье.
            Не откладывайте лечение, звоните прямо сейчас. Мы работаем круглосуточно в Москве.</p>
          <p class="lor-info__subtitle pb-6">
            тел.: <a class="tel" href="#"> 8 (495) 266-28-73 </a> (круглосуточно)
          </p>
        </div>
      </section>
    </div>
</div>
</template>

<style scoped>

</style>
