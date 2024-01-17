<script setup lang='ts'>
const award:any[] = [
  {
    id: 1,
    img: 'https://lorlor.ru/images/p641071.jpg',
    title: '"Клиника уха, горла и носа" в ТОП-30 частных клиник Москвы',
    subtitle: 'Премия Продокторов по мнению пациентов.',
    date: '01.11.21'
  },
  {
    id: 2,
    img: 'https://lorlor.ru/images/p606743.jpg',
    title: 'Наша Клиника получила "Звезду Качества" за лучшее предприятие страны 2020 года.',
    subtitle: '',
    date: '01.02.21'
  }
]
const news:any[] = [
  {
    img: 'https://lorlor.ru/images/p687267.jpg',
    title: 'Открытие филиала "Клиники уха, горла и носа" в Сочи состоится 31 июля',
    subtitle: 'Мы открываем новый филиал в городе Сочи.'
  }
]
const element:any[] = [
  {
    id: 1,
    img: 'https://lorlor.ru/images/p687307.jpg',
    title: 'Зависимость от сосудосуживающих капель: последствия',
    subtitle: 'Выпуск № 2 о сосудосуживающих препаратах от оториноларинголога Алексея Васильева.',
    date: '25.07.23'
  },
  {
    id: 2,
    img: 'https://lorlor.ru/images/p687307.jpg',
    title: 'Зависимость от сосудосуживающих капель: последствия',
    subtitle: 'Выпуск № 2 о сосудосуживающих препаратах от оториноларинголога Алексея Васильева.',
    date: '21.07.23'
  },
  {
    id: 3,
    img: 'https://lorlor.ru/images/p687283.jpg',
    title: 'Капли VS спрей',
    subtitle: 'Что подойдет именно вам? Рассказывает отоларинголог клиники - Анатолий Якушев.',
    date: '18.07.23'
  },
  {
    id: 4,
    img: 'https://lorlor.ru/images/p561247.jpg',
    title: 'Когда необходимо делать пункцию?',
    subtitle: 'Об этом рассказал Акопян Карен - отоларинголог клиники.',
    date: '14.07.23'
  },
  {
    id: 5,
    img: 'https://lorlor.ru/images/p687252.jpg',
    title: 'Для чего необходимо слухопротезирование?',
    subtitle: 'Как проходит процедура в нашей клинике? Смотрите в новом ролике.',
    date: '11.07.23'
  },
  {
    id: 6,
    img: 'https://lorlor.ru/images/p687241.jpg',
    title: 'Ребенок боится врачей?',
    subtitle: 'Что с этим делать - рассказывает на видео наш оториноларинголог Рагим Садыхов.',
    date: '07.07.23'
  },
  {
    id: 7,
    img: 'https://lorlor.ru/images/p687213.jpg',
    title: 'Эпизодически кружится голова?',
    subtitle: 'Какое обследование показано при периодически возникающих головокружениях?',
    date: '04.07.23'
  },
  {
    id: 8,
    img: 'https://lorlor.ru/images/p687212.jpg',
    title: '3 способа остановить кровь из носа',
    subtitle: 'Видео для тех, кто не разбивал носы в детстве, а теперь столкнулся с такой проблемой, как носовое кровотечение!',
    date: '27.06.23'
  },
  {
    id: 9,
    img: 'https://lorlor.ru/images/p687176.jpg',
    title: 'С нами легко, даже если вы приехали оперироваться из другой страны!',
    subtitle: 'Развенчиваем основные вопросы, которые могут мешать принятию решения.',
    date: '20.06.23'
  }
]
const video:any[] = [
  {
    id: 1,
    img: '/img/ci1155057v480x320s0.jpg.png',
    title: 'Букет на завтрак: чем полезен салат из роз?',
    subtitle: 'Наш врач-эндокринолог, диетолог Севастьянова Наталья готовит салат из лепестков роз в прямом эфире.',
    date: ''
  },
  {
    id: 2,
    img: '/img/ci2v480x320s0.jpg',
    title: 'Исследование слуха методом КСВП под наркозом?',
    subtitle: '',
    date: ''
  },
  {
    id: 3,
    img: '/img/ci3v480x320s0.jpg',
    title: 'Аденоиды: лечить или удалять?',
    subtitle: '',
    date: ''
  },
  {
    id: 4,
    img: '/img/ci4v480x320s0.jpg',
    title: 'Как побороть нафтизиновую зависимость?',
    subtitle: '',
    date: ''
  },
  {
    id: 5,
    img: '/img/ci5v480x320s0.jpg',
    title: 'Доктор Никонов ждет вас и готов помочь!',
    subtitle: '',
    date: ''
  },
  {
    id: 6,
    img: '/img/ci6v480x320s0.jpg',
    title: 'Антивозрастные стратегии на страже здоровья и красоты. Пошаговые...',
    subtitle: 'Вебинар от врача-диетолога, эндокринолога Севастьяновой Натальи Владимировны.',
    date: ''
  },
  {
    id: 7,
    img: '/img/ci7v480x320s0.jpg',
    title: 'Что такое аденоиды, почему они воспаляются и как проводится аденотомия',
    subtitle: '',
    date: ''
  },
  {
    id: 8,
    img: '/img/ci8v480x320s0.jpg',
    title: 'Все о гайморотомии',
    subtitle: '',
    date: ''
  },
  {
    id: 9,
    img: '/img/ci9v480x320s0.jpg',
    title: 'Тонзилэктомия',
    subtitle: '',
    date: ''
  }
]
const article:any[] = [
  {
    id: 1,
    img: 'https://lorlor.ru/images/p686835v1920x1080s0.jpg',
    title: 'Аденоиды - все о заболевании',
    subtitle: 'Что такое аденоиды, причины, симптомы, степени гипертрофии, методы диагностики и лечения аденоидов.',
    date: ''
  },
  {
    id: 2,
    img: 'https://lorlor.ru/images/ci1143680v480x320s0.jpg',
    title: 'Синдром пустого носа',
    subtitle: 'Все о губительном для качества жизни заболевании.',
    date: ''
  },
  {
    id: 3,
    img: 'https://lorlor.ru/images/ci1143420v480x320s0.jpg',
    title: 'Фурункул наружного слухового прохода',
    subtitle: 'Фурункул уха - болезненное воспаление волосяного мешочка слухового канала. Симптомы, анатомия и лечение.',
    date: ''
  },
  {
    id: 4,
    img: '/img/ci11v480x320s0.jpg',
    title: 'Тиннитус (звон в ушах): все о беспокоящем симптоме',
    subtitle: 'Глубинные причины возникновения в связи с анатомией человека, влияние на психику, грамотный подход к лечению.',
    date: ''
  },
  {
    id: 5,
    img: '/img/ci12v480x320s0.jpg',
    title: 'Фармакотерапия никотиновой зависимости',
    subtitle: 'Препараты для лечения табачной зависимости.',
    date: ''
  },
  {
    id: 6,
    img: '/img/ci13v480x320s0.jpg',
    title: 'Спирометрия - что это и зачем она нужна?',
    subtitle: 'Спирометрия - базисный метод функциональной диагностики внешнего дыхания.',
    date: ''
  },
  {
    id: 7,
    img: '/img/ci14v480x320s0.jpg',
    title: 'Слизь в горле или синдром постназального затекания',
    subtitle: 'В этой статье объясняются симптомы и причины слизи в носоглотке, а также способы диагностики и лечения.',
    date: ''
  },
  {
    id: 8,
    img: '/img/ci15v480x320s0.jpg',
    title: 'Экссудативный средний отит у детей. Симптомы, причины и лечение',
    subtitle: 'Негнойное заболевание среднего уха, при котором в среднем ухе происходит накопление патологической жидкости.',
    date: ''
  },
  {
    id: 9,
    img: 'https://lorlor.ru/images/ci1105933v480x320s0.jpg',
    title: 'Синдром Маршалла (PFAPA синдром)',
    subtitle: 'Что такое синдром Маршалла, клиническая картина, симптомы, лечение.',
    date: ''
  }
]
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
const products = ref([
  {
    title: 'Поможем услышать мир',
    subtitle: 'Лучшие лор хирурги',
    link: 'Узнайне подробнее >>',
    image: '/img/operation-new1.jpg'
  },
  {
    title: 'Лор операция',
    subtitle: 'Лучшие лор хирурги',
    link: 'Узнайне подробнее >>',
    image: '/img/rev_column_bg.png'
  }, {
    title: 'Лор операция',
    subtitle: 'Лучшие лор хирурги',
    link: 'Узнайне подробнее >>',
    image: '/img/operation-new1.jpg'
  }, {
    title: 'Лор операция',
    subtitle: 'Лучшие лор хирурги',
    link: 'Узнайне подробнее >>',
    image: '/img/rev_column_bg.png'
  }
])
const position = ref('center')
const visible = ref(false)

const openPosition = (pos:any) => {
  position.value = pos
  visible.value = true
}
</script>
<template>
  <div>
    <!--    ==============================products__slider=====================================-->
    <section class="products mb-8">
      <Carousel
        :value="products"
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
    <!--    ==============================products__slider=====================================-->
    <!--=======================================services=======================================-->
    <section class="mb-8 ">
      <div class="container">
        <div class="grid">
          <div class="col-12 md:col-4 lg:col-3 mb-5 ">
            <div class="services ">
              <div class="services-info border-bottom-2 border-300 py-1">
                <div class="services-menu-title">
                  <img class="icon-icon" src="../public/img/cardiogram.svg" alt="">
                  <h1 class="services__tittle">
                    ДИАГНОСТИКА
                  </h1>
                </div>
              </div>
              <ul class="menu__group">
                <li><a class="services__subtitle" href="#">Тимпанометрия</a></li>
                <li><a class="services__subtitle" href="#">Аудиометрия</a></li>
                <li><a class="services__subtitle" href="#">Электрокохлеография</a></li>
                <li><a class="services__subtitle" href="#">Эндоскопия носа</a></li>
                <li><a class="services__subtitle" href="#">КТ пазух носа</a></li>
                <li><a class="services__subtitle" href="#">КТ челюсти</a></li>
              </ul>
            </div>
          </div>
          <div class="col-12 md:col-4 lg:col-3 mb-5">
            <div class="services ">
              <div class="services-info border-bottom-2 border-300 py-1">
                <div class="services-menu-title">
                  <img class="icon-icon" src="../public/img/syringe.svg" alt="">
                  <h1 class="services__tittle">
                    ПРОЦЕДУРЫ
                  </h1>
                </div>
              </div>
              <ul class="menu__group">
                <li><a class="services__subtitle" href="#">Промывание носа</a></li>
                <li><a class="services__subtitle" href="#">Пункция пазух</a></li>
                <li><a class="services__subtitle" href="#">Ямик</a></li>
                <li><a class="services__subtitle" href="#">Промывание миндалин</a></li>
                <li><a class="services__subtitle" href="#">Удаление серной пробки</a></li>
              </ul>
            </div>
          </div>
          <div class="col-12 md:col-4 lg:col-3 mb-5">
            <div class="services ">
              <div class="services-info border-bottom-2 border-300 py-1">
                <div class="services-menu-title">
                  <img class="icon-icon" src="../public/img/blood-transfusion.svg" alt="">
                  <h1 class="services__tittle">
                    ОПЕРАЦИИ
                  </h1>
                </div>
              </div>
              <ul class="menu__group">
                <li><a class="services__subtitle" href="#">Удаление миндалин</a></li>
                <li><a class="services__subtitle" href="#">Удаление аденоидов</a></li>
                <li><a class="services__subtitle" href="#">Септопластика</a></li>
                <li><a class="services__subtitle" href="#">Удаление полипов</a></li>
                <li><a class="services__subtitle" href="#">Тимпанопластика</a></li>
              </ul>
            </div>
          </div>
          <div class="col-12 md:col-4 lg:col-3 mb-5">
            <div class="services ">
              <div class="services-info border-bottom-2 border-300 py-1">
                <div class="services-menu-title">
                  <img class="icon-icon" src="../public/img/hospital-1.svg" alt="">
                  <h1 class="services__tittle">
                    КЛИНИКА
                  </h1>
                </div>
              </div>
              <ul class="menu__group">
                <li><a class="services__subtitle" href="#">О клинике</a></li>
                <li><a class="services__subtitle" href="#">Специалисты</a></li>
                <li><a class="services__subtitle" href="#">Детский лор-врач</a></li>
                <li><a class="services__subtitle" href="#">Лор-врач на дом</a></li>
                <li><a class="services__subtitle" href="#">Контакты</a></li>
              </ul>
            </div>
          </div>
          <Button label=" Все услуги..." severity="" outlined @click="openPosition('bottom')"></Button>
          <Dialog v-model:visible="visible" class="dialog" :style="{ width: '100vw', height: '100vh', background: 'rgba(80, 101, 169, 0.95)' }" :position="position" :modal="true" :draggable="false">
            <div class="grid">
              <div class="col-12 md:col-4 lg:col-3 mb-5 ">
                <div class="services-all">
                  <div class="services-info border-bottom-2 border-300 py-1">
                      <h1 class="services__tittle services__tittle--dialog">
                        ДИАГНОСТИКА
                      </h1>
                    </div>
                  <ul class="menu__group menu__group--dialog">
                    <li><a class="services__subtitle" href="#">Эндоскопия носа</a></li>
                    <li><a class="services__subtitle" href="#">КТ пазух носа</a></li>
                    <li><a class="services__subtitle" href="#">Тимпономерия</a></li>
                    <li><a class="services__subtitle" href="#">Аудиометрия</a></li>
                  </ul>
                  <h1 class="services__tittle services__tittle--dialog-txt">Исследования уха</h1>
                  <ul class="menu__group menu__group--dialog">
                    <li><a class="services__subtitle" href="#">Исследование проходимости слуховой трубы</a></li>
                    <li><a class="services__subtitle" href="#">Аудиометрия</a></li>
                    <li><a class="services__subtitle" href="#">Отоскопия</a></li>
                    <li><a class="services__subtitle" href="#">Камертональное исследование</a></li>
                    <li><a class="services__subtitle" href="#">Электрокохлеография</a></li>
                    <li><a class="services__subtitle" href="#">КТ височной кости</a></li>
                    <li><a class="services__subtitle" href="#">Диагностика вестибулярной функции</a></li>
                  </ul>
                  <h1 class="services__tittle services__tittle--dialog-txt">Исследования носа и пазух</h1>
                  <ul class="menu__group menu__group--dialog">
                    <li><a class="services__subtitle" href="#"> Эндоскопия носа</a></li>
                    <li><a class="services__subtitle" href="#">Риноскопия</a></li>
                    <li><a class="services__subtitle" href="#">Диафаноскопия</a></li>
                    <li><a class="services__subtitle" href="#">УЗИ пазух носа</a></li>
                    <li><a class="services__subtitle" href="#">Рентгенография пазух</a></li>
                    <li><a class="services__subtitle" href="#">Компьютерная томография пазух</a></li>
                    <li><a class="services__subtitle" href="#">Зондирование пазух</a></li>
                  </ul>
                  <h1 class="services__tittle services__tittle--dialog-txt">Исследования глотки, гортани</h1>
                  <ul class="menu__group menu__group--dialog">
                    <li><a class="services__subtitle" href="#">Пальпация</a></li>
                    <li><a class="services__subtitle" href="#">Ларингоскопия</a></li>
                    <li><a class="services__subtitle" href="#">Рентгенография гортан</a></li>
                    <li><a class="services__subtitle" href="#">Диагностика голосовой функции</a></li>
                  </ul>
                </div>
              </div>
              <div class="col-12 md:col-4 lg:col-3 mb-5">
                <div class="services-all ">
                  <div class="services-info border-bottom-2 border-300 py-1">
                      <h1 class="services__tittle services__tittle--dialog">
                        ПРОЦЕДУРЫ
                      </h1>
                  </div>
                  <ul class="menu__group menu__group--dialog">
                    <li><a class="services__subtitle" href="#">Промывание носа</a></li>
                    <li><a class="services__subtitle" href="#">Пункция пазух</a></li>
                    <li><a class="services__subtitle" href="#">Ямик</a></li>
                    <li><a class="services__subtitle" href="#">Промывание миндалин</a></li>
                    <li><a class="services__subtitle" href="#">Удаление серной пробки</a></li>
                    <li><a class="services__subtitle" href="#">Лазеротерапия</a></li>
                    <li><a class="services__subtitle" href="#">Электрофорез</a></li>
                    <li><a class="services__subtitle" href="#">Тампонада носа</a></li>
                    <li><a class="services__subtitle" href="#">Прижигание слизистой носа</a></li>
                    <li><a class="services__subtitle" href="#">Удаление инородных тел из носа</a></li>
                    <li><a class="services__subtitle" href="#">Милта</a></li>
                    <li><a class="services__subtitle" href="#">Кварц</a></li>
                    <li><a class="services__subtitle" href="#">Соляная пещера</a></li>
                  </ul>

                </div>
              </div>
              <div class="col-12 md:col-4 lg:col-3 mb-5">
                <div class="services-all ">
                  <div class="services-info border-bottom-2 border-300 py-1">
                      <h1 class="services__tittle services__tittle--dialog">
                        ОПЕРАЦИИ
                      </h1>
                    </div>
                  <ul class="menu__group menu__group--dialog">
                    <li><a class="services__subtitle" href="#">Удаление миндалин</a></li>
                    <li><a class="services__subtitle" href="#">Удаление аденоидов</a></li>
                    <li><a class="services__subtitle" href="#">Септопластика</a></li>
                    <li><a class="services__subtitle" href="#">Удаление полипов</a></li>
                    <li><a class="services__subtitle" href="#">Тимпанопластика</a></li>
                  </ul>
                  <h1 class="services__tittle services__tittle--dialog-txt">
                    Операции носа и пазух носа
                  </h1>
                <ul class="menu__group menu__group--dialog">
                  <li><a class="services__subtitle" href="#">Риносептопластика</a></li>
                  <li><a class="services__subtitle" href="#">Вазотомия</a></li>
                  <li><a class="services__subtitle" href="#">Полисинусотомия</a></li>
                  <li><a class="services__subtitle" href="#">Конхотомия носовых раковин</a></li>
                  <li><a class="services__subtitle" href="#">Резекция носовой перегородки</a></li>
                  <li><a class="services__subtitle" href="#">Пункция верхнечелюстной пазухи</a></li>
                </ul>
                  <h1 class="services__tittle services__tittle--dialog-txt">
                   Операции уха
                  </h1>
                  <ul class="menu__group menu__group--dialog">
                    <li><a class="services__subtitle" href="#">Стапедопластика</a></li>
                    <li><a class="services__subtitle" href="#">Мирингопластика</a></li>
                    <li><a class="services__subtitle" href="#">Мастоидопластика</a></li>
                    <li><a class="services__subtitle" href="#"> Шунтирование барабанной полости</a></li>
                  </ul>
                  <h1 class="services__tittle services__tittle--dialog-txt">
                    Операции глотки и гортани
                  </h1>
                  <ul class="menu__group menu__group--dialog">
                  <li><a class="services__subtitle" href="#">Тонзиллэктомия</a></li>
                  <li><a class="services__subtitle" href="#">Удаление голосовых связок</a></li>
                  <li><a class="services__subtitle" href="#">Трахеостомия</a></li>
                  </ul>
                  <h1 class="services__tittle services__tittle--dialog-txt">
                    Прочее
                  </h1>
                  <ul class="menu__group menu__group--dialog">
                    <li><a class="services__subtitle" href="#">Подготовка к операции</a></li>
                    <li><a class="services__subtitle" href="#">Лор-хирурги</a></li>
                    <li><a class="services__subtitle" href="#">Рассрочка по операциям</a></li>
                  </ul>
                </div>
                </div>
              <div class="col-12 md:col-4 lg:col-3 mb-5">
                <div class="services-all ">
                  <div class="services-info border-bottom-2 border-300 py-1">
                      <h1 class="services__tittle services__tittle--dialog">
                        КЛИНИКА
                      </h1>
                    </div>
                  <ul class="menu__group menu__group--dialog">
                    <li><a class="services__subtitle" href="#">О клинике</a></li>
                    <li><a class="services__subtitle" href="#">Специалисты</a></li>
                    <li><a class="services__subtitle" href="#">Детский лор-врач</a></li>
                    <li><a class="services__subtitle" href="#">Лор-врач на дом</a></li>
                    <li><a class="services__subtitle" href="#">Контакты</a></li>
                    <li><a class="services__subtitle" href="#">Оборудование</a></li>
                    <li><a class="services__subtitle" href="#">Операционная</a></li>
                    <li><a class="services__subtitle" href="#">Стационар</a></li>
                    <li><a class="services__subtitle" href="#">Фото клиники</a></li>
                    <li><a class="services__subtitle" href="#">Видео</a></li>
                  </ul>
                  <h1 class="services__tittle services__tittle--dialog-txt">
                    Филиалы:
                  </h1>
                <ul class="menu__group menu__group--dialog">
                  <li><a class="services__subtitle" href="#"> На "Цветном бульваре"</a></li>
                  <li><a class="services__subtitle" href="#">На "Преображенской площади"</a></li>
                  <li><a class="services__subtitle" href="#"> На "Бульваре Дмитрия Донского"</a></li>
                  <li><a class="services__subtitle" href="#">На "Мичуринском проспекте"</a></li>
                  <li><a class="services__subtitle" href="#">На "Фили"</a></li>
                </ul>
                <h1 class="services__tittle services__tittle--dialog-txt">
                  Прочие направления
                </h1>
              <ul class="menu__group menu__group--dialog">
                <li><a class="services__subtitle" href="#">Слухопротезирование</a></li>
                <li><a class="services__subtitle" href="#">Терапия</a></li>
                <li><a class="services__subtitle" href="#">Педиатрия</a></li>
                <li><a class="services__subtitle" href="#">УЗИ сосудов</a></li>
                <li><a class="services__subtitle" href="#">УЗИ сердца</a></li>
                <li><a class="services__subtitle" href="#">Неврология</a></li>
                <li><a class="services__subtitle" href="#">Мануальная терапия</a></li>
                <li><a class="services__subtitle" href="#">Аллергология-иммунология</a></li>
                <li><a class="services__subtitle" href="#">Кардиология</a></li>
              </ul>
              <h1 class="services__tittle services__tittle--dialog-txt">
                Пациентам:
              </h1>
            <ul class="menu__group menu__group--dialog">
              <li><a class="services__subtitle" href="#">Контроль качества</a></li>
              <li><a class="services__subtitle" href="#"> Отзывы о лор-клинике</a></li>
            </ul>
                </div>
              </div>
            </div>
          </Dialog>
        </div>
      </div>
    </section>
    <!--=======================================services=======================================-->
    <!--=====================================information__title===============================-->
    <section>
      <div class="container">
        <div class="lor-info">
          <h1 class="lor-info__title">
            Лор-клиника
          </h1>
          <p class="lor-info__subtitle">
            Клиника уха, горла и носа является современной специализированной лор-клиникой в Москве, способной оказывать своевременную высококвалифицированную медицинскую помощь пациентам с заболеваниями уха, горла и носа всех возрастных категорий, используя самые современные технологии.
          </p>
          <p class="lor-info__subtitle">
            В нашей клинике доступна востребованная услуга - реабилитация после ковида. Мы составили комплекс эффективных лечебных процедур, направленных на полнейшее восстановление всех ресурсов организма после перенесенной инфекции.
          </p>
          <p class="lor-info__subtitle">
            Своевременное обращение к врачу поможет сохранить Ваше здоровье.
            Не откладывайте лечение, звоните прямо сейчас. Мы работаем круглосуточно в Москве.
          </p>
          <p class="lor-info__subtitle">
            тел.: <a class="tel" href="#">8 (495) 153-04-49</a> (круглосуточно)
          </p>
        </div>
      </div>
    </section>
    <!--=====================================information__title===============================-->
    <!--======================================specialists=====================================-->
    <section class="bg-gray-100 pt-20">
      <div class="container">
        <h1 class="main-title main-title--card mb-4">
          Наши специалисты
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
        <div class="flex justify-content-center">
          <Button class="border-noround mr-3 border-0 p-tag-primary bg-cyan-700 hover:bg-cyan-600 text-xl" label="Задать вопрос врачу" />
          <Button class="border-noround ml-5 text-blue-700 hover:bg-blue-700 hover:text-white text-xl" label="Все специалисты" severity="success" outlined />
        </div>
        <p class="main-description mt-5 pb-6">
          Наши лор-врачи
          имеют огромный и уникальный опыт лечения лор-заболеваний, как взрослых пациентов, так и детей. У нас работает высокопрофессиональная команда отоларингологов высшей квалификационной категории, ринохирургов и отохирургов, в том числе 40% наших врачей имеют ученую степень кандидата медицинских наук. Наши специалисты ежедневно решают сложнейшие задачи и проводят уникальные
          хирургические операции
          лор-органов.
        </p>
      </div>
    </section>
    <!--======================================specialists=====================================-->
    <!--======================================equipment=====================================-->
    <section>
      <div class="equipment">
        <div class="container">
          <h1 class="title">
            Современное оборудование
          </h1>
          <p class="lor__txt">
            Мы оснащены современным оборудованием, которое позволяет проводить качественную диагностику заболеваний уха, горла и носа, в том числе эндоскопический осмотр лор-органов, УЗИ пазух носа,
            <a href="#">КТ пазух носа</a>, аудиометрию и многое другое. Качественная диагностика пациентов является ключевым фактором эффективного лечения, позволяет выявлять лор-патологии на ранней стадии и проводить своевременное и эффективное лечение.
          </p>
          <img class="equipment__img" src="https://lorlor.ru/content/images/equipment.jpg" alt="fffffffff">
          <h1 class="title pb-4">
            Детский лор
          </h1>
          <p class="lor__txt">
            Профилактика и <span>лечение лор-заболеваний у детей</span> является одним из наших основных профилей деятельности. Клиника приспособлена для приема самых маленьких пациентов, современное медицинское оборудование оснащено специальными средствами для оказания медицинской помощи детям (например, специальные детские насадки для эндоскопического оборудования и т.п.).
            <a href="#">Детские лор-врачи</a> клиники имеют огромный опыт лечения детей всех возрастных категорий, обладают специальными навыками общения с детьми и способны оказать своевременную и высококвалифицированную медицинскую помощь, учитывая возрастные особенности диагностики и лечения ребенка.
          </p>
          <h1 class="title pb-4">
            Лор-врач круглосуточно
          </h1>
          <p class="lor__txt">
            Клиника уха, горла и носа работает 24 часа в сутки 7 дней в неделю. Наш филиал на "Цветном бульваре" не закрывается ни на минуту и готов принять пациентов в любое время суток. В клинике всегда присутствует
            <a href="#">дежурный лор-врач</a>, готовый оказать своевременную медицинскую помощь нашим пациентам.
          </p>
          <h1 class="title pb-4">
            Вызов лор-врача на дом
          </h1>
          <p class="lor__txt">
            Для удобства наших пациентов в клинике организована <a href="#">служба вызова лор-врача на дом</a>. В случае если у Вас температура или Вы по объективным причинам не можете самостоятельно посетить клинику, свяжитесь с администратором клиники и вызовите лор-врача на дом. Прием заявок осуществляется круглосуточно.
          </p>
          <h1 class="title">
            Операции в клинике уха, горла и носа
          </h1>
          <p class="lor__txt">
            В клинике проводится широкий спектр <a href="#">хирургических операций</a>, таких как <a
              href="#"
            >удаление аденоидов, удаление миндалин, тимпанопластика, септопластика</a>, ринопластика, вазотомия и др. В нашем распоряжении операционная и стационар, которые оснащены самым современным медицинским оборудованием. Команда хирургов представлена широким спектром специалистов своей области, имеющих огромный опыт проведения сложнейших хирургических операций с использованием современных технологий оперирования и реабилитации пациентов.
          </p>
          <img class="img" src="https://lorlor.ru/content/images/surgery/adenoidy.jpg" alt="ffffff">
          <h1 class="title pb-4">
            Центр лор-помощи в Москве
          </h1>
          <p class="lor__txt">
            Клиника уха, горла и носа является современным <span>лор-центром в Москве </span>, где каждый человек может рассчитывать на высококвалифицированную медицинскую помощь, пройти курсы физиотерапии и укрепить свое здоровье.
          </p>
          <p class="lor__txt">
            В клинике физиотерапевтические процедуры включают в себя целый спектр мероприятий:
          </p>
          <ul>
            <li class="li">
              <a class="a" href="#">лазеротерапия</a>  и магнитотерапия на аппарате Милта
            </li>
            <li class="li">
              <a class="a" href="#">тубус кварц</a>
            </li>
            <li class="li">
              пневмомассаж
            </li>
            <li class="li">
              <a class="a" href="#">электрофорез</a>
            </li>
            <li class="li">
              промывание лакун миндалин на аппарате «Тонзиллор»
            </li>
            <li class="li">
              <a class="a" href="#">соляная пещера</a>
            </li>
          </ul>
          <p class="lor__txt">
            Физиотерапия является неотъемлемой частью комплексной терапии, позволяет достигать более быстрых результатов в лечении заболеваний лор-органов. Также физиотерапия позволяет сократить сроки реабилитации в послеоперационном периоде.
          </p>
        </div>
      </div>
    </section>
    <!--======================================equipment=====================================-->
    <!--======================================awards=====================================-->
    <section class="awards bg-[#f2f2f2] pt-7">
      <div class="container">
        <h1 class="title pb-4">
          Наши награды
        </h1>
        <div class="grid">
          <div v-for="item in award" :key="item.id" class="col-12 sm:col-6 lg:col-4">
            <Card class="h-full">
              <template #header>
                <div style="height: 300px">
                  <img class="w-full h-full object-cover" alt="user header" :src="item.img" style="border-bottom: 3px solid #5bbdbe">
                </div>
              </template>
              <template #title>
                {{ item.title }}
              </template>
              <template #subtitle>
                {{ item.subtitle }}
              </template>
              <template #content>
                <p>
                  {{ item.date }}
                </p>
              </template>
            </Card>
          </div>
        </div>
      </div>
    </section>
    <!--======================================awards=====================================-->
    <!--   ==================================news=====================================-->
    <section class="news bg-[#f2f2f2] pt-7">
      <div class="container">
        <h1 class="title">
          Новости клиники
        </h1>
        <div class="grid">
          <div v-for="item in news" :key="item.id" class=" col-12 sm:col-6 lg:col-4">
            <Card class="h-full">
              <template #header>
                <div style="height: 300px">
                  <img class="w-full h-full object-cover" alt="user header" :src="item.img" style="border-bottom: 3px solid #5bbdbe">
                </div>
              </template>
              <template #title>
                {{ item.title }}
              </template>
              <template #subtitle>
                {{ item.subtitle }}
              </template>
              <template #content>
                <p>
                  {{ item.date }}
                </p>
              </template>
            </Card>
          </div>
        </div>
        <div class="grid">
          <div v-for="item in element" :key="item.id" class=" col-12 sm:col-6 lg:col-4 mt-3">
            <Card class="h-full w-full">
              <template #header>
                <div style="height: 300px">
                  <img class="w-full h-full object-cover" alt="user header" :src="item.img" style="border-bottom: 3px solid #5bbdbe">
                </div>
              </template>
              <template #title>
                {{ item.title }}
              </template>
              <template #subtitle>
                {{ item.subtitle }}
              </template>
              <template #content>
                <p>
                  {{ item.date }}
                </p>
              </template>
            </Card>
          </div>
        </div>
        <div class="flex align-items-center justify-content-center">
          <button class="button font">
            Все новости
          </button>
        </div>
      </div>
    </section>
    <!--    ==========================news=====================================-->
    <!--    ==============================video====================================-->
    <section class="video bg-[#f2f2f2] pt-7">
      <div class="container">
        <h1 class="title">
          Видео
        </h1>
        <div class="grid">
          <div v-for="item in video" :key="item.id" class=" col-12 sm:col-6 lg:col-4 mt-3">
            <Card class="h-full">
              <template #header>
                <div style="height: 300px">
                  <img class="w-full h-full object-cover" alt="user header" :src="item.img" style="border-bottom: 3px solid #5bbdbe">
                </div>
              </template>
              <template #title>
                {{ item.title }}
              </template>
              <template #subtitle>
                {{ item.subtitle }}
              </template>
              <template #content>
                <p>
                  {{ item.date }}
                </p>
              </template>
            </Card>
          </div>
        </div>
        <div class="flex align-items-center justify-content-center">
          <button class="button font">
            Все видео
          </button>
        </div>
      </div>
    </section>
    <!--    ==============================video====================================-->
    <!--  ============================================================================-->
    <section class="articles bg-[#f2f2f2] pt-7">
      <div class="container">
        <h1 class="title">
          Статьи
        </h1>
        <div class="grid">
          <div v-for="item in article" :key="item.id" class=" col-12 sm:col-6 lg:col-4">
            <Card class="h-full">
              <template #header>
                <div style="height: 300px">
                  <img class="w-full h-full object-cover" alt="user header" :src="item.img" style="border-bottom: 3px solid #5bbdbe">
                </div>
              </template>
              <template #title>
                {{ item.title }}
              </template>
              <template #subtitle>
                {{ item.subtitle }}
              </template>
              <template #content>
                <p>
                  {{ item.date }}
                </p>
              </template>
            </Card>
          </div>
        </div>
        <div class="flex align-items-center justify-content-center">
          <button class="button font">
            Все статьи
          </button>
        </div>
      </div>
    </section>
    <!--  ===========================Symptoms===============================================-->
    <section class="symptoms">
      <div class="container">
        <div class="title">
          Симптомы заболеваний
        </div>
        <div class="grid">
          <div class="col-12 md:col-6 lg:col-3 mb-5 ">
            <div class="block">
              <div class="block-info border-bottom-2 border-300 py-1">
                <div class="block-menu-title">
                  <h1 class="block__tittle mt-6">
                    Уши
                  </h1>
                </div>
              </div>
              <ul class="menu__group">
                <li><a class="block__subtitle" href="#">Шум в ухе</a></li>
                <li><a class="block__subtitle" href="#">Снижение слуха</a></li>
                <li><a class="block__subtitle" href="#">Боль в ухе</a></li>
                <li><a class="block__subtitle" href="#">Серная пробка в ухе</a></li>
                <li><a class="block__subtitle" href="#">Заложенность уха</a></li>
                <li><a class="block__subtitle" href="#">Выделения из уха</a></li>
                <li><a class="block__subtitle" href="#">Экзостозы</a></li>
                <li><a class="block__subtitle" href="#">Травмы уха</a></li>
                <li><a class="block__subtitle" href="#">Ушной свищ</a></li>
                <li><a class="block__subtitle" href="#">Кровь из уха</a></li>
                <li><a class="block__subtitle" href="#">Атрезии слухового прохода</a></li>
              </ul>
            </div>
          </div>
          <div class="col-12 md:col-6 lg:col-3 mb-5 ">
            <div class="block">
              <div class="block-info border-bottom-2 border-300 py-1">
                <div class="block-menu-title">
                  <h1 class="block__tittle mt-6">
                    ГОРЛО
                  </h1>
                </div>
              </div>
              <ul class="menu__group">
                <li><a class="block__subtitle" href="#">Боль в горле</a></li>
                <li><a class="block__subtitle" href="#">Увеличенные миндалины</a></li>
                <li><a class="block__subtitle" href="#">Кашель</a></li>
                <li><a class="block__subtitle" href="#">Першение в горле</a></li>
                <li><a class="block__subtitle" href="#">Налет на языке</a></li>
                <li><a class="block__subtitle" href="#">Пропал голос</a></li>
                <li><a class="block__subtitle" href="#">Отек гортани</a></li>
                <li><a class="block__subtitle" href="#">Аденоиды</a></li>
              </ul>
            </div>
          </div>
          <div class="col-12 md:col-6 lg:col-3 mb-5 ">
            <div class="block">
              <div class="block-info border-bottom-2 border-300 py-1">
                <div class="block-menu-title">
                  <h1 class="block__tittle mt-6">
                    ГОРЛО
                  </h1>
                </div>
              </div>
              <ul class="menu__group">
                <li><a class="block__subtitle" href="#">Кровотечение из носа</a></li>
                <li><a class="block__subtitle" href="#">Полипы в носу</a></li>
                <li><a class="block__subtitle" href="#">Насморк</a></li>
                <li><a class="block__subtitle" href="#">Заложенность носа</a></li>
                <li><a class="block__subtitle" href="#">Кривой нос</a></li>
                <li><a class="block__subtitle" href="#">Фурункул в носу</a></li>
                <li><a class="block__subtitle" href="#">Перфорация носовой перегородки</a></li>
                <li><a class="block__subtitle" href="#">Травмы носа</a></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!--  =================================diseases===========================================-->
    <section class="diseases">
      <div class="container">
        <div class="title">
          Заболевания лор-органов
        </div>
        <div class="grid">
          <div class="col-12 md:col-6 lg:col-3 mb-5 ">
            <div class="block">
              <div class="block-info border-bottom-2 border-300 py-1">
                <div class="block-menu-title">
                  <h1 class="block__tittle mt-6">
                    Болезни носа
                  </h1>
                </div>
              </div>
              <ul class="menu__group">
                <li><a class="block__subtitle" href="#">Синусит</a></li>
                <li><a class="block__subtitle" href="#">Гайморит</a></li>
                <li><a class="block__subtitle" href="#">Фронтит</a></li>
                <li><a class="block__subtitle" href="#">Этмоидит</a></li>
                <li><a class="block__subtitle" href="#">Сфеноидит</a></li>
                <li><a class="block__subtitle" href="#">Ринит</a></li>
                <li><a class="block__subtitle" href="#">Ринофима</a></li>
                <li><a class="block__subtitle" href="#">Озена</a></li>
                <li><a class="block__subtitle" href="#">Гранулематоз Вегенера</a></li>
                <li><a class="block__subtitle" href="#">Сикоз носа</a></li>
                <li><a class="block__subtitle" href="#">Атрезия хоан</a></li>
              </ul>
            </div>
          </div>
          <div class="col-12 md:col-6 lg:col-3 mb-5 ">
            <div class="block">
              <div class="block-info border-bottom-2 border-300 py-1">
                <div class="block-menu-title">
                  <h1 class="block__tittle mt-6">
                    Болезни горла
                  </h1>
                </div>
              </div>
              <ul class="menu__group">
                <li><a class="block__subtitle" href="#">Ларингит</a></li>
                <li><a class="block__subtitle" href="#">Тонзиллит</a></li>
                <li><a class="block__subtitle" href="#">Паратонзиллярный абсцесс</a></li>
                <li><a class="block__subtitle" href="#">Фарингит</a></li>
                <li><a class="block__subtitle" href="#">Трахеит</a></li>
                <li><a class="block__subtitle" href="#">Ложный круп</a></li>
                <li><a class="block__subtitle" href="#">Хондроперихондрит</a></li>
                <li><a class="block__subtitle" href="#">Заглоточный абсцесс</a></li>
              </ul>
            </div>
          </div>
          <div class="col-12 md:col-6 lg:col-3 mb-5 ">
            <div class="block">
              <div class="block-info border-bottom-2 border-300 py-1">
                <div class="block-menu-title">
                  <h1 class="block__tittle mt-6">
                    Болезни уха
                  </h1>
                </div>
              </div>
              <ul class="menu__group">
                <li><a class="block__subtitle" href="#">Отит</a></li>
                <li><a class="block__subtitle" href="#">Отосклероз</a></li>
                <li><a class="block__subtitle" href="#">Болезнь Меньера</a></li>
                <li><a class="block__subtitle" href="#">Тубоотит</a></li>
                <li><a class="block__subtitle" href="#">Лабиринтит</a></li>
                <li><a class="block__subtitle" href="#">Нейросенсорная тугоухость</a></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>
