<template>
  <div class="contacts">
  <section>
    <hr>
  <div class="container">
    <div>
      <Breadcrumb class="p-component--crumbing ml--4" :home="home" :model="items" />
    </div>
    <h1 class="font-semibold text-5xl pb-4">
      Контакты
    </h1>
    <div class="grid">
      <div class="col-12 md:col-6">
        <p class="text-xl font-medium">Единый контактный телефон:</p>
        <p class="lor-info__subtitle pb-4">
          <a class="tel" href="#"> 8 (495) 266-28-72 </a> (круглосуточно)
        </p>
        <p class="text-xl font-medium">Инстаграм:</p>
        <div class="flex">
          <div class="">
          <p class="lor-info__subtitle pb-4">
            <a class="tel" href="#">lorlor.ru</a>
          </p>
          </div>
          <div class="pt-2 pl-2 pb-5"><a href="https://www.instagram.com/"><img src="https://lorlor.ru/content/Images/inst.png" style="height: 20px; width: 100%" alt=""></a></div></div>
        <p class="text-xl font-medium">Обратная связь</p>
        <Button label="Напишите нам" class="border-noround bg-indigo-600" raised/>
      </div>
      <div class="col-12 md:col-6">
        <p class="text-xl font-medium">Электронная почта:</p>
        <p class="lor-info__subtitle pb-4">
          <a class="tel" href="#"> info@lorlor.ru </a>
        </p>
        <p class="text-xl font-medium">ТикТок:</p>
        <div class="flex">
          <div>
          <p class="lor-info__subtitle">
            <a class="tel" href="#">lorlor.ru</a>
          </p>
          </div>
          <div class="pt-1 pl-2 pb-5"><a href="https://www.tiktok.com/"><img src="https://download.logo.wine/logo/TikTok/TikTok-Logo.wine.png" style="height:30px; width: 100%;" alt=""></a></div>
        </div>
      </div>
      <div class="col-12 md:col-6">
        <h1 class="font-semibold text-5xl mb-6 mt-6 ">Филиалы</h1>
        <ul>
          <li class="li__lor pb-5">
            <router-link class=" text-xl font-light" to="">
              <p class="tel1">Филиал на Цветном бульваре</p>
            </router-link>
          </li>
          <li class="li__lor pb-5">
            <router-link class=" text-xl  font-light" to="/list">
              <p class="tel2">Филиал на Преображенской площади</p>
            </router-link>
          </li>
          <li class="li__lor pb-5">
            <router-link class=" text-xl  text-black font-light " to="/list">
              <p class="tel3">Филиал на бульваре Дмитрия Донского</p>
            </router-link>
          </li>
          <li class="li__lor pb-5">
            <router-link class=" text-xl  text-black font-light " to="/list">
              <p class="tel4">Филиал на Мичуринском проспекте</p>
            </router-link>
          </li>
          <li class="li__lor pb-5">
            <router-link class=" text-xl  text-black font-light " to="/list">
              <p class="tel5">Филиал на Фили</p>
            </router-link>
          </li>
        </ul>
      </div>
    </div>
    <h1 class="font-semibold text-5xl pb-4">
      Адреса филиалов:
    </h1>
 <router-link to="">
    <div class="branch ml--6">
      <div class="branch__metro grey" />
      <div class="branch-info">
        <h1 class="branch__tittle">
          Цветной бульвар
        </h1>
        <p class="branch__subtitle">
          Москва, Самотечная, 5
        </p>
        <p class="branch__subtitle mb-4">
          (Круглосуточна)
        </p>
      </div>
    </div>
 </router-link>
    <a class="tel1 " href="#">Подробнее</a>
    <div class="block__map mt-4">
      <iframe
          class="map"
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2300421.7626201552!2d71.0852738873337!3d39.98560333131973!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38bc35b99dc9f579%3A0x4590139fc0c83acb!2z0J3QvtC-0LrQsNGC!5e0!3m2!1sru!2skg!4v1683379402356!5m2!1sru!2skg"
          style="border: 0; width: 100%; height: 60vh;"
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
      ></iframe>
    </div>
    <h1 class="font-semibold text-5xl pb-4 pt-5">
      Как пройти:
    </h1>
    <p class="lor__txt">Выход из метро Цветной бульвар, первый вагон из центра. Выйдя из метро идете налево, по
      ул. Цветной бульвар.
      Проходите прямо 2 светофора (пройдёте под Садовым кольцом), перед Вами будет бульвар, который надо обойти слева и
      выйти на улицу Самотечная. Переходите на другую сторону Самотечной улицы (см. карту) и идете вдоль нее от Садового
      кольца. Третий дом от Садового кольца - ул. Самотечная, д.5</p>
    <div class="block__map"><iframe width="" height="500" src="https://www.youtube.com/embed/aUMdFbxxHnA" style="width: 100%" title="Цветной бульвар - дорога от метро" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe></div>
    <h1 class="font-semibold text-5xl pb-4 pt-5">
      Парковка
    </h1>
    <p class="text-xl pt-2 pb-2">Около клиники есть платная парковка.</p>
    <p class="text-xl font-medium pt-2">График работы:</p>
    <p style="background-color: #f2f2f2; width: 170px; margin-bottom: 30px">Пн. - Вс. с 09:00 до 21:00</p>
    <router-link to="">
    <div class="branch ml--6 ">
      <div class="branch__metro red" />
      <div class="branch-info">
        <h1 class="branch__tittle">
          Преображенская площадь
        </h1>
        <p class="branch__subtitle">
          Москва, Б. Черкизовская, 5
        </p>
        <p class=" branch__txt mb-4">
          Ежедневно c 09:00 до 21:00
        </p>
      </div>
    </div>
    </router-link>
    <a class="tel1 " href="#">Подробнее</a>
    <div class="block__map mt-4">
      <iframe
          class="map"
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2300421.7626201552!2d71.0852738873337!3d39.98560333131973!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38bc35b99dc9f579%3A0x4590139fc0c83acb!2z0J3QvtC-0LrQsNGC!5e0!3m2!1sru!2skg!4v1683379402356!5m2!1sru!2skg"
          style="border: 0; width: 100%; height:60vh;"
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
      ></iframe>
    </div>
    <h1 class="font-semibold text-5xl pb-4 pt-5">
      Как пройти:
    </h1>
    <p class="lor__txt">Станция метро "Преображенская площадь", первый вагон из центра, из стеклянных дверей налево, по правой лестнице поднимаетесь на улицу и идете прямо до конца здания к магазину Эверест, переходите дорогу, сразу поворачиваете налево, идете по Малой Черкизовской (200 метров) и поворачиваете направо на улицу Страховская, второй дом справа - это наше двухэтажное здание желтого цвета, на входе вывеска "Медицинский центр".</p>
    <div class="block__map">
      <iframe width="" height="500" src="https://www.youtube.com/embed/aUMdFbxxHnA" style="width: 100%" title="Цветной бульвар - дорога от метро" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
    </div>
    <h1 class="font-semibold text-5xl pb-4 pt-5">
      Парковка
    </h1>
    <p class="text-xl pt-2 pb-2">Около клиники есть платная парковка.</p>
    <p class="text-xl font-medium pt-2">График работы:</p>
    <p style="background-color: #f2f2f2; width: 170px; margin-bottom: 30px">Пн. - Вс. с 09:00 до 21:00</p>
   <router-link to="">
     <div class="branch ml--6">
       <div class="branch__metro grey" />
       <div class="branch-info">
         <h1 class="branch__tittle">
           Бульвар Дмитрия Донского
         </h1>
         <p class="branch__subtitle">
           Москва, Грина, 28 корпус 1
         </p>
         <p class="branch__txt mb-4">
           Ежедневно c 09:00 до 21:00
         </p>
       </div>
     </div>
   </router-link>
    <a class="tel1 " href="#">Подробнее</a>
    <div class="block__map mt-4">
      <iframe
          class="map"
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2300421.7626201552!2d71.0852738873337!3d39.98560333131973!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38bc35b99dc9f579%3A0x4590139fc0c83acb!2z0J3QvtC-0LrQsNGC!5e0!3m2!1sru!2skg!4v1683379402356!5m2!1sru!2skg"
          style="border: 0; width: 100%; height: 60vh;"
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
      ></iframe>
    </div>
    <h1 class="font-semibold text-5xl pb-4 pt-5">
      Как пройти:
    </h1>
    <p class="lor__txt">Выход из метро Цветной бульвар, первый вагон из центра. Выйдя из метро идете налево, по
      ул. Цветной бульвар.
      Проходите прямо 2 светофора (пройдёте под Садовым кольцом), перед Вами будет бульвар, который надо обойти слева и
      выйти на улицу Самотечная. Переходите на другую сторону Самотечной улицы (см. карту) и идете вдоль нее от Садового
      кольца. Третий дом от Садового кольца - ул. Самотечная, д.5</p>
    <div class="block__map"><iframe width="" height="500" src="https://www.youtube.com/embed/w2ikGLH78B4" style="width: 100%" title="Цветной бульвар - дорога от метро" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe></div>
    <h1 class="font-semibold text-5xl pb-4 pt-5">
      Парковка
    </h1>
    <p class="text-xl pt-2 pb-2">Около клиники есть платная парковка.</p>
    <p class="text-xl font-medium pt-2">График работы:</p>
    <p style="background-color: #f2f2f2; width: 170px; margin-bottom: 60px">Пн. - Вс. с 09:00 до 21:00</p>
    <router-link to="">
      <div class="branch ml--6">
        <div class="branch__metro yellow" />
        <div class="branch-info">
          <h1 class="branch__tittle">
            Мичуринский проспект
          </h1>
          <p class="branch__subtitle">
            Москва, Грина, 28 корпус 1
          </p>
          <p class="branch__txt mb-4">
            Ежедневно c 09:00 до 21:00
          </p>
        </div>
      </div>
    </router-link>
    <a class="tel1 " href="#">Подробнее</a>
    <div class="block__map mt-4">
      <iframe
          class="map"
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2300421.7626201552!2d71.0852738873337!3d39.98560333131973!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38bc35b99dc9f579%3A0x4590139fc0c83acb!2z0J3QvtC-0LrQsNGC!5e0!3m2!1sru!2skg!4v1683379402356!5m2!1sru!2skg"
          style="border: 0; width: 100%; height: 60vh;"
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
      ></iframe>
    </div>
    <h1 class=" text-2xl font-medium pb-4 pt-5">
      Как пройти:
    </h1>
    <ul class="lor-ul">
      <li class="mt12px color-#F45B69 li">
        <router-link class="text-xl text-black font-light" to="/list">
          <span class="font-medium">«Кунцевская»</span> – маршрутка №308м или №459.
        </router-link>
      </li>
      <li class="mt12px color-#F45B69 li">
        <router-link class="text-xl text-black font-light" to="/list">
          <span class="font-medium">«Юго-Западная»</span> – маршрутки №629м, №308м, №519 или автобус №688.
        </router-link>
      </li>
      <li class="mt12px color-#F45B69 li">
        <router-link class="text-xl text-black font-light" to="/list">
          <span class="font-medium">«Раменки»</span> – автобусом 120(7 остановок) до остановки «Управа района Очаково-
          <br> Матвеевское» или пешком 15 мин.
        </router-link>
      </li>
      <li class="mt12px color-#F45B69 li">
        <router-link class="text-xl text-black font-light" to="/list">
          <span class="font-medium">«Мичуринский проспект»</span> – маршрутка №308м или №459.
        </router-link>
      </li>
      <li class="mt12px color-#F45B69 li">
        <router-link class="text-xl text-black font-light" to="/list">
          <span class="font-medium">«Озерная»</span> – автобусами 329 или С17 (6 остановок) до остановки «Управа района
          Очаково-Матвеевское».
        </router-link>
      </li>
    </ul>
    <p class="text-xl font-medium pt-4">График работы:</p>
    <p style="background-color: #f2f2f2; width: 200px; margin-bottom: 60px" class="text-xl mb-3">Пн. - Вс. с 09:00 до
      21:00</p>
    <router-link to="">
      <div class="branch ml--6">
        <div class="branch__metro blue" />
        <div class="branch-info">
          <h1 class="branch__tittle">
            Фили
          </h1>
          <p class="branch__subtitle">
            Москва, Береговой проезд, 7
          </p>
          <p class="branch__txt mb-4">
            Ежедневно c 09:00 до 21:00
          </p>
        </div>
      </div>
    </router-link>
    <a class="tel1 " href="#">Подробнее</a>
    <div class="block__map mt-4">
      <iframe
          class="map"
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2300421.7626201552!2d71.0852738873337!3d39.98560333131973!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x38bc35b99dc9f579%3A0x4590139fc0c83acb!2z0J3QvtC-0LrQsNGC!5e0!3m2!1sru!2skg!4v1683379402356!5m2!1sru!2skg"
          style="border: 0; width: 100%; height: 60vh;"
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
      ></iframe>
    </div>
    <p class="text-xl font-medium pt-4">Как пройти:</p>
    <p class="text-xl">Проезд от станций метро:</p>
    <p class="lor__txt">Станция метро Фили, первый вагон из центра, из стеклянных дверей прямо, перейти по
      пешеходному
      переходу через улицу Новозаводская в сторону автобусной остановки.</p>
    <p class="lor__txt">На автобусной остановке автобус 653. Ехать до остановки «Береговой проезд» (3-я
      остановка).</p>
    <p class="text-xl font-medium pt-2">График работы:</p>
    <p style="background-color: #f2f2f2; width: 200px; margin-bottom: 60px;" class="text-xl font-light">Пн. - Вс. с
      09:00 до 21:00</p>
  </div>
  </section>
  <section>
  <div class="container">
    <h1 class="text-5xl font-medium">Реквизиты для оплаты</h1>
    <p class="text-xl font-semibold bg-gray-300">Данные об организации</p>
    <p class="text-xl font-light bg-gray-300 pr-4 pt-1 pb-1"><span class="pr-4">Наименование Организации:</span>ООО «Клиника УГН»</p>
    <p class="text-xl font-light"><span class="pr-4">Наименование Организации:</span>ООО «Клиника УГН»</p>
    <p class="text-xl font-light bg-gray-300 pt-1 pb-1"><span class="pr-4">Наименование:</span>ООО «Клиника УГН»</p>
    <p class="text-xl font-light"><span class="pr-4">Почтовый адрес</span>127473, Москва, ул.Самотечная, д.5</p>
    <p class="text-xl font-light bg-gray-300 pt-1 pb-1"><span class="pr-4">Почтовый адрес</span>О127473, Москва, ул.Самотечная, д.5</p>
    <p class="text-xl font-light"><span class="pr-4">ФИО Генерального директора</span>Халитова Ирина Каримовна</p>
    <p class="text-xl font-light bg-gray-300 pt-1 pb-1"><span class="pr-4">ФИО Главного бухгалтера</span>Халитова Ирина Каримовна</p>
    <p class="text-xl font-light "><span class="pr-4">Телефон клиники</span>8-495-764-33-03</p>
    <p class="text-xl font-light bg-gray-300 pt-1 pb-1  "><span class="pr-4">График работы</span>круглосуточно</p>
    <p class="text-xl font-light"><span class="pr-4">Наименование Организации:</span>ООО «Клиника УГН»</p>
    <h1 class="text-xl font-medium pt-4" style="width: 335px">Реквизиты для оплаты</h1>
    <p class="text-xl font-semibold bg-gray-300" style="width: 335px">Банковские реквизиты организации</p>
    <p class="text-xl font-light pr-4 pt-1 pb-1" style="width: 335px"><span class="pr-4">БИК</span>30101810200000000700</p>
    <p class="text-xl font-light bg-gray-300" style="width: 335px"><span class="pr-4" >Р/С</span>40702810900000186955</p>
    <p class="text-xl font-light pb-5"><span class="pr-4" style="width: 335px">НАЗВАНИЕ БАНКА</span>АО "Райффайзенбанк"</p>
    <p class="text-xl font-light">Своевременное обращение к врачу поможет сохранить Ваше здоровье.</p>
    <p class="text-xl font-light">Не откладывайте лечение, звоните прямо сейчас. Мы работаем круглосуточно в Москве.</p>
    <p class="text-xl pb-5"><span class="text-blue-800 tel text-3xl">8 (495) 153-05-88</span>(круглосуточно)</p>

  </div>
  </section>
  </div>
</template>
<script lang="ts" setup>
const home = ref({
  label: 'Главная',
  to: '/'
})
const items = ref([
  { label: 'О клинике' }
])
</script>
