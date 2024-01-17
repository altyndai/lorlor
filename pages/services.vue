<template>
  <section id="list">
    <div class="container">
      <div>
        <Breadcrumb class="p-component--crumbing" :home="home" :model="items" />
      </div>
      <div class="grid mt-8">
        <div class="col-12 md:col-6  xl:col-4 scroll-hover">
          <div class="service flex line-scroll justify-content-center md:justify-content-start">
            <img class="w-4rem" src="../public/img/cardiogram.svg" alt="">
            <h1 class="list-title ml-4">
              ДИАГНОСТИКА
            </h1>
          </div>
          <ul class="list-menu list-menu--services">
            <h6 class="flex text-1.2rem font-sans ml--6">
              Исследования уха
            </h6>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Акустическая импедансометрия</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Аудиометрия</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Вызов лор-врача на дом - второй пациент по одному адресу</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Вызов лор-врача на дом в Москве</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Игровая тональная аудиометрия</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Исследование функции слуховых труб</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Компьютерная томография околоносовых пазух</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Консультация врача по выбору чек-апа</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">КСВП – обследование слуха</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Отоакустическая эмиссия (ОАЭ) для обследования слуха</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Первичный прием лор-врача</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Пункционная биопсия под контролем УЗИ-аппарата экспертного класса</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Сурдолог в Москве</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Сурдологический комплекс</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Тест на коронавирус за сутки - экспресс анализ на COVID-19</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Тимпанометрия</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">УЗИ сердца</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">УЗИ сосудов</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">УЗИ сосудов головы</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">УЗИ сосудов шеи</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Ультразвуковое исследование (УЗИ)</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Электрокохлеография</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Эндоскопия носа</NuxtLink></li>
            <h6 class="text-1.2rem font-sans ml--6">Исследование проходимости слуховой трубы</h6>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Аудиометрия</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Диагностика вестибулярной функции</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Игровая тональная аудиометрия</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Камертональное исследование</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">КТ височной кости</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Отоскопия</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Сурдолог в Москве</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Сурдологический комплекс</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Тренировка слуховых труб</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Электрокохлеография</NuxtLink></li>
            <h6 class="text-1.2rem font-sans ml--6">Исследования носа и пазух</h6>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Диагностика дыхательной функции носа</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Зондирование пазух</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Компьютерная томография пазух</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Лечение гиперосмии (в т.ч. после коронавируса)</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Лечение гипосмии (в т.ч. после коронавируса)</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Лечение какосмии (в т.ч. после коронавируса)</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Лечение обонятельных галлюцинаций (в т.ч. после коронавируса)</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Лечение паросмии (в т.ч. после коронавируса)</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Риноскопия</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">УЗИ пазух носа</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Эндоскопическое обследование носа у детей при помощи гибкого эндоскопа</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Эндоскопия носа</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Эндоскопия носа ригидным эндоскопом</NuxtLink></li>
            <h6 class="text-1.2rem font-sans ml--6">Исследования глотки, гортани</h6>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Диагностика голосовой функции</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Ларингоскопия</NuxtLink></li>
            <li class="list-item"><p class=""></p><NuxtLink class="list-link" to="">Пальпация гортани и шеи</NuxtLink></li>
          </ul>
        </div>
        <div class="col-12 md:col-6  xl:col-4 scroll-hover">
          <div>
            <div class="service flex line-scroll justify-content-center md:justify-content-start">
              <img class="w-4rem" src="https://lorlor.ru/content/images/icons/videocall.svg" alt="videocall">
              <h1 class="list-title ml-4">ОНЛАЙН-КОНСУЛЬТАЦИЯ</h1>
            </div>
            <ul class="list-menu list-menu--services mb-7">
              <li class="list-item"><NuxtLink class="list-link" to="">Онлайн-консультация лор-врача</NuxtLink></li>
              <li class="list-item"><NuxtLink class="list-link" to="">Памятка: как получить консультацию онлайн</NuxtLink></li>
            </ul>
          </div>
          <div class="service flex line-scroll justify-content-center md:justify-content-start">
            <img class="w-4rem" src="../public/img/syringe.svg" alt="">
            <h1 class="list-title ml-4">
              ПРОЦЕДУРЫ
            </h1>
          </div>
          <ul class="list-menu list-menu--services mb-7">
            <li class="list-item"><NuxtLink class="list-link" to="">Вакуумное промывание лакун миндалин аппаратом «Тонзиллор»</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Видеонистагмография (ВНГ)</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Кварц</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Компрессионный ингалятор «Пари Синус» (Pari Sinus)</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Лазеротерапия</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Магнитотерапия</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">МИЛТА</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Прижигание слизистой носа</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Промывание миндалин</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Промывание носа методом перемещения</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Промывание уха из-за серной пробки</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Реабилитация после COVID-19</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Сдача анализов</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Тампонада носа</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Тренировка слуховых труб</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Удаление инородных тел из носа</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Целенаправленные комплексы</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Электрофорез</NuxtLink></li>
          </ul>
          <div class="service flex line-scroll justify-content-center md:justify-content-start">
            <img class="w-4rem" src="../public/img/cardiogram.svg" alt="">
            <h1 class="list-title ml-3">ПРОЧИЕ УСЛУГИ</h1>
          </div>
          <ul class="list-menu list-menu--services">
            <li class="list-item"><NuxtLink class="list-link" to="">Аллергология и иммунология</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Анализ на пищевую непереносимость: тест и диагностика</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Бронхиолит: симптомы и лечение</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Бронхоэктазия: симптомы и лечение</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Идиопатический легочный фиброз: симптомы и лечение</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Интерстициальный пневмофиброз: симптомы и лечение</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Кардиология</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Легочная гипертензия: симптомы и лечение</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Лечение аллергического конъюнктивита: симптомы и причины</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Лечение аллергического поллиноза (аллергия на пыльцу)</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Лечение аллергического ринита: симптомы и причины</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Лечение аллергической крапивницы: симптомы и причины</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Лечение атопического дерматита: причины и рекомендации</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Лечение бронхиальной астмы: симптомы и причины</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Лечение пищевой аллергии: симптомы и рекомендации</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Лечение рецидивирующего герпеса</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Лечение фурункулеза: причины и профилактика</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Мануальная терапия</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Массаж</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Неврология</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Педиатрия</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Справка об отсутствии COVID-19 на английском языке</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Стационар</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Терапия</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Тромбоэмболия легочной артерии: симптомы и лечение</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Хроническая обструктивная болезнь легких: симптомы и лечение</NuxtLink></li>
          </ul>
        </div>
        <div class="col-12 md:col-6  xl:col-4 scroll-hover">
          <div class="service flex line-scroll justify-content-center md:justify-content-start">
            <img class="w-4rem" src="../public/img/blood-transfusion%20(1).svg" alt="">
            <h1 class="list-title ml-4">
              ОПЕРАЦИИ
            </h1>
          </div>
          <ul class="list-menu list-menu--services">
            <h6 class="flex md:hidden text-1.2rem font-sans ml--6">
              Операции носа и пазух носа
            </h6>
            <li class="list-item"><NuxtLink class="list-link" to="">Госпитальный скрининг</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Септопластика</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Тимпанопластика барабанной перепонки</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Удаление аденоидов современными методами</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Удаление миндалин</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Удаление полипов в носу</NuxtLink></li>
            <h6 class="flex text-1.2rem font-sans ml--6">Операции носа и пазух носа</h6>
            <li class="list-item"><NuxtLink class="list-link" to="">Аденотомия</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Вазотомия</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Гайморотомия</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Инфундибулотомия</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Конхотомия (турбинопластика) носовых раковин</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Перфорация носовой перегородки</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Полипотомия</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Полисинусотомия</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Пункция верхнечелюстной пазухи</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Резекция носовой перегородки</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Репозиция костей носа</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Сфенотомия</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Удаление кисты в пазухе носа</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Удаление кисты в пазухе носа</NuxtLink></li>
            <h6 class="flex text-1.2rem font-sans ml--6">Операции уха</h6>
            <li class="list-item"><NuxtLink class="list-link" to="">Мастоидопластика</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Мирингопластика</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Отопластика</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Перфорация барабанной перепонки</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Слухопротезирование</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Стапедопластика</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Тимпанопластика барабанной перепонки</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Шунтирование барабанной перепонки</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Шунтирование барабанной перепонки</NuxtLink></li>
            <h6 class="flex text-1.2rem font-sans ml--6">Операции глотки и гортани</h6>
            <li class="list-item"><NuxtLink class="list-link" to="">Аденотомия</NuxtLink></li>
            <li class="list-item"><NuxtLink class="list-link" to="">Тонзиллэктомия</NuxtLink></li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const home = ref({
  label: 'Главная',
  to: '/'
})
const items = ref([
  { label: 'Услуга' }
])
</script>

<style scoped>
</style>
