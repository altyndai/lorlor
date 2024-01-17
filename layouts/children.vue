<script setup lang="ts">
import { useThemeStore } from '../stores'
const themeStore = useThemeStore()
const items = ref([
  {
    label: 'Главная',
    to: '/'
  },
  {
    label: 'Детский лор',
    to: '/childrens-lor'
  },
  {
    label: 'Лор-врачи',
    to: '/doctors/doctors'
  },
  {
    label: 'Лор-операции',
    to: '/operation'
  },
  {
    label: 'Услуги',
    to: '/services'
  },
  {
    label: 'Цены',
    to: '/price'
  },
  {
    label: 'Пациенту',
    items: [
      [
        {
          label: 'Setting 1',
          items: [{ label: 'Setting 1.1' }, { label: 'Setting 1.2' }]
        },
        {
          label: 'Setting 2',
          items: [{ label: 'Setting 2.1' }, { label: 'Setting 2.2' }]
        },
        {
          label: 'Setting 3',
          items: [{ label: 'Setting 3.1' }, { label: 'Setting 3.2' }]
        }
      ],
      [
        {
          label: 'Technology 4',
          items: [{ label: 'Setting 4.1' }, { label: 'Setting 4.2' }]
        }
      ]
    ]
  },
  {
    label: 'Контакты',
    to: '/contacts'
  }
])
</script>

<template>
  <div>
    <!-- header   -->
    <header>
      <div>
        <div class="container">
          <div class="line-box border-bottom-1 border-300 py-1 bg-[#FFF]">
            <div class="flex justify-content-between align-items-centers">
              <Menubar :model="items" />

              <div class="flex align-items-center ">
                <Button
                    class="ml-3"
                    icon="pi pi-user text-2xl"
                    severity="secondary"
                    rounded
                    aria-label="Bookmark"
                    text
                />
                <Button
                    class="ml-3"
                    icon="pi pi-eye text-2xl"
                    severity="secondary"
                    rounded
                    aria-label="Bookmark"
                    text
                />
                <Button
                    class="ml-3"
                    icon="pi pi-search text-2xl"
                    severity="secondary"
                    rounded
                    aria-label="Bookmark"
                    text
                />
                <div class="line" />
                <a href="tel:8(495)266-28-74" class="ml-4 text-pink-500 font-medium text-xl">8 (495) 266-28-74</a>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div>
        <div class="container">
          <div class="grid justify-content-center">
            <div class="col-12 md:col-4 lg:col mb-5 mt-4">
              <div class="branch">
                <img class="logo" src="https://lorlor.ru/content/images/logo-kids.svg">
              </div>
            </div>
            <div class="col-12 md:col-4 lg:col mb-5 mt-4">
              <div class="branch">
                <div class="branch__metro grey" />
                <div class="branch-info">
                  <h1 class="branch__tittle">
                    Цветной бульвар
                  </h1>
                  <p class="branch__subtitle">
                    Москва, Самотечная, 5
                  </p>
                  <Tag class="branch__tag" value="Круглосуточно" />
                </div>
              </div>
            </div>
            <div class="col-12 md:col-4 lg:col mb-5 mt-4">
              <div class="branch">
                <div class="branch__metro red" />
                <div class="branch-info">
                  <h1 class="branch__tittle">
                    Преображенская площадь
                  </h1>
                  <p class="branch__subtitle">
                    Москва, Б. Черкизовская, 5
                  </p>
                  <p class=" branch__txt">
                    Ежедневно c 09:00 до 21:00
                  </p>
                </div>
              </div>
            </div>
            <div class="col-12 md:col-4 lg:col mb-5 mt-4">
              <div class="branch">
                <div class="branch__metro grey" />
                <div class="branch-info">
                  <h1 class="branch__tittle">
                    Бульвар Дмитрия Донского
                  </h1>
                  <p class="branch__subtitle">
                    Москва, Грина, 28 корпус 1
                  </p>
                  <p class="branch__txt">
                    Ежедневно c 09:00 до 21:00
                  </p>
                </div>
              </div>
            </div>
            <div class="col-12 md:col-4 lg:col mb-5 mt-4">
              <div class="branch">
                <div class="branch__metro yellow" />
                <div class="branch-info">
                  <h1 class="branch__tittle">
                    Мичуринский проспект
                  </h1>
                  <p class="branch__subtitle">
                    Москва, Грина, 28 корпус 1
                  </p>
                  <p class="branch__txt">
                    Ежедневно c 09:00 до 21:00
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </header>
    <Link rel="stylesheet" :href="themeStore.link" />
    <slot />
    <!--  footer  -->
    <footer class="bg-[#364779] pt-8 pb-7">
      <div class="container">
        <div class="grid justify-content-between">
          <div class="col-12 lg:col-7">
            <div class="grid">
              <div class="col-12 sm:col-6 md:col-4 mb-4">
                <h2 class="footer-title">
                  Клиника
                </h2>
                <ul class="footer-menu">
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      О клинике
                    </router-link>
                  </li>
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      Специалисты
                    </router-link>
                  </li>
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      Контакты
                    </router-link>
                  </li>
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      Работа в клинике
                    </router-link>
                  </li>
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      Новости
                    </router-link>
                  </li>
                </ul>
              </div>
              <div class="col-12 sm:col-6 md:col-4 mb-4">
                <h2 class="footer-title">
                  Услуги
                </h2>
                <ul class="footer-menu">
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      Прайс-лист
                    </router-link>
                  </li>
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      Детский лор
                    </router-link>
                  </li>
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      Дежурный лор
                    </router-link>
                  </li>
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      Лор-врач на дом
                    </router-link>
                  </li>
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      Онлайн-консультация
                    </router-link>
                  </li>
                </ul>
              </div>
              <div class="col-12 sm:col-6 md:col-4 mb-4">
                <h2 class="footer-title">
                  Пациентам
                </h2>
                <ul class="footer-item">
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      Контроль качества
                    </router-link>
                  </li>
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      Отзывы о лор-клинике
                    </router-link>
                  </li>
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      Статьи
                    </router-link>
                  </li>
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      Клинические случаи
                    </router-link>
                  </li>
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      Прием по ДМС
                    </router-link>
                  </li>
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      Налоговый вычет
                    </router-link>
                  </li>
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      Бесплатное лечение
                    </router-link>
                  </li>
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      Партнеры
                    </router-link>
                  </li>
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      Отзывы на картах
                    </router-link>
                  </li>
                  <li class="footer-item">
                    <router-link class="footer-link" to="">
                      Публичная оферта о компьютерной диагностике слуха
                    </router-link>
                  </li>
                </ul>
              </div>
            </div>
            <div class="flex-column">
              <h2 class="footer-title">
                Конфиденциальность
              </h2>
              <p class="footer-link">
                Согласие на обработку персональных данных
              </p>
              <p class="footer-link">
                Политика в отношении обработки персональных данных
              </p>
            </div>
          </div>
          <div class="col-12 lg:col-3">
            <div class="flex justify-content-center ">
              <div class="grid--branch-footer relative grid sm:justify-content-center my-5 flex-column">
                <div class="branch-animation-left" />
                <div class="col-12 ">
                  <div class="branch flex-column">
                    <a href="tel:8(495)153-04-49" class=" text-white font-bold text-3xl" style="width: fit-content">8 (495) 153-04-49</a>
                    <p class="text-white text-1.1em">
                      (круглосуточно)
                    </p>
                  </div>
                </div>
                <div class="col-12">
                  <div class="branch branch--white-text flex">
                    <div class="mr-3">
                      <img src="/img/sun.svg" alt="sun" class="w-2rem">
                    </div>
                    <div>
                      <div class="flex align-items-center">
                        <h3 class="branch__title text-white">
                          г. Сочи
                        </h3>
                        <Tag value="cкоро" class="text-sm font-normal p-tag-danger ml-2 -mt-4" />
                      </div>
                      <p class="branch__subtitle text-white mb-1">
                        Навагинская, 7
                      </p>
                      <p class="branch__subtitle text-white">
                        Ежедневно c 09:00 до 20:00
                      </p>
                    </div>
                  </div>
                </div>
                <div class="branch-animation-right" />
              </div>
            </div>
          </div>
        </div>
        <div class="footer-icons ml--8">
          <div class="footer-icon">
            <img src="https://lorlor.ru/Content/images/Zen_shortlogo.svg" alt="dssadsda" class="w-7rem h-5rem">
          </div>
          <div class="footer-icon">
            <img src="https://lorlor.ru/Content/images/iconmonstr-vk-1.svg" alt="dwdas" class="w-3rem">
          </div>
          <div class="footer-icon">
            <i class="pi pi-youtube text-5xl" />
          </div>
          <div class="footer-icon">
            <i class="pi pi-instagram text-3xl" />
          </div>
          <div class="footer-icon">
            <i class="pi pi-telegram text-3xl" />
          </div>
        </div>
      </div>
      <div class="bg-[#465B9C] w-full py-6">
        <p class="text-[#d4d4d4] text-0.9em text-center font-sans">
          © 2013 - 2023 Клиника уха, горла и носа, лицензия №ЛО-77-01-0099047 от 24.09.2014г.
        </p>
        <p class="text-[#d4d4d4] text-0.9em text-center font-sans">
          Создание сайта клиники и медицинский маркетинг: medmarketing
        </p>
        <p class="text-[#d4d4d4] text-0.9em text-center font-sans">
          Карта сайта
        </p>
      </div>
    </footer>
  </div>
</template>
