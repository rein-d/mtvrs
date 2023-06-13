<template>
  <div class="w-full">
    <!-- Hero section -->
    <section id="hero" class="w-full pb-24">
      <BaseSection>
        <div class="col-span-12 lg:col-span-6 mt-12 xl:mt-10 space-y-4 sm:space-y-6 px-6 text-center sm:text-left">
          <span data-aos="fade-right" data-aos-once="true" class="text-base text-gradient font-semibold uppercase"
            >Метавселенной называют всё подряд, чтобы приобщиться к хайпу</span
          >
          <h1
            data-aos="fade-right"
            data-aos-once="true"
            class="text-[2.5rem] sm:text-5xl xl:text-6xl font-bold leading-tight capitalize sm:pr-8 xl:pr-10"
          >
            Что же такое <span class="text-header-gradient">МЕТАВСЕЛЕННАЯ</span> Сейчас?
          </h1>
          <p data-aos="fade-down" data-aos-once="true" data-aos-delay="300" class="paragraph hidden sm:block">
            Масштабируемая и совместимая сеть 3D-виртуальных миров, визуализируемых в реальном времени, которые могут быть доступны синхронно и постоянно практически неограниченному числу пользователей с индивидуальным ощущением присутствия и непрерывностью данных, таких как личность, история, права, объекты, коммуникации и платежи.
          </p>
        </div>
        <div class="hidden sm:block col-span-12 lg:col-span-6">
          <div class="w-full">
            <img
              data-aos="fade-up"
              data-aos-once="true"
              :src="require('~/assets/img/hero-image.webp')"
              class="-mt-4"
              alt=""
            />
          </div>
        </div>
        <img
          data-aos="fade-up"
          data-aos-delay="300"
          :src="require('~/assets/img/pattern/ellipse-1.png')"
          class="hidden sm:block absolute bottom-12 xl:bottom-16 left-4 xl:left-0 w-6"
        />
        <img
          data-aos="fade-up"
          data-aos-delay="300"
          :src="require('~/assets/img/pattern/ellipse-2.png')"
          class="hidden sm:block absolute top-4 sm:top-10 right-68 sm:right-96 xl:right-[32rem] w-6"
        />
        <img
          data-aos="fade-up"
          data-aos-delay="300"
          :src="require('~/assets/img/pattern/star.png')"
          class="hidden sm:block absolute top-20 sm:top-28 right-16 lg:right-0 lg:left-[30rem] w-8"
        />
      </BaseSection>
    </section>

    <!-- Buy and trade section -->
    <section class="w-full my-24">
      <BaseSection>
        <LandingBuyTradeImage class="sm:hidden mb-8" />
        <div class="col-span-12 lg:col-span-5 space-y-6 px-4 sm:px-6 mt-20">
          <h2 class="text-4xl font-semibold">
            Новая эра <br class="hidden sm:block" />
            Технологического развития
          </h2>
          <br>
          <span class="text-base text-gradient font-semibold uppercase">
            Глубокая интеграция физического и цифрового мира
          </span>
          <div class="space-y-6 lg:pr-12">
            <p>Метавселенная — это виртуальное пространство, которое создает симуляцию реальности и объединяет существующие сервисы, контент, продукты брендов в единой среде.</p>
            <p>Пользователи могут взаимодействовать друг с другом и с цифровыми объектами через свои аватары, с помощью персональных компьютеров, а также используя специальные гарнитуры, очки и шлемы.</p>
          </div>
        </div>
        <LandingBuyTradeImage data-aos="fade-left" class="hidden sm:block" />
      </BaseSection>
    </section>

    <!-- Partners section -->
    <section class="bg-partner relative max-w-full sm:mx-6 my-24 shadow sm:rounded-2xl overflow-hidden">
      <div class="w-full px-6 sm:px-0 py-16 flex flex-col items-center justify-center space-y-4 text-center">
        <h3 data-aos="flip-down" class="text-[2.2rem] sm:text-4xl xl:text-5xl font-bold leading-tight sm:pr-8 xl:pr-10">
          Проведем в Метавселенную!</h3>
        <div data-aos="fade-up" class="flex flex-wrap items-center justify-center">
          <LandingPartnerImage
            v-for="img in ['rusmetaverse.png', 'MetaVersoshnaya.png', 'DAOLAW.png']"
            :key="img"
            :img="img"
          />
        </div>
      </div>
    </section>

    <!-- Credit card section -->
    <section class="w-full my-36">
      <BaseSection data-aos="fade-down">
        <div class="col-span-12 lg:col-span-7">
          <div class="w-full">
            <img :src="require('~/assets/img/section3.png')" class="w-[95%]" alt="" />
          </div>
        </div>
        <div class="col-span-12 lg:col-span-5 space-y-6 px-4 sm:px-6 mt-20">
          <h2 class="text-4xl font-semibold">
            Как устроена <span class="text-header-gradient">Метавселенная</span>
          </h2>
          <p class="paragraph">Концепций метавселенной много, но самая известная принадлежит венчурному инвестору Мэтью Болу. В своем представлении Бол приводит семь характеристик другого мира:</p>
          <ul class="space-y-4 sm:space-y-2">
            <LandingListItem title="Метавселенная не прекращается: ее нельзя поставить на паузу, стереть или завершить" />
            <LandingListItem title="Все события внутри вселенной происходят в режиме реального времени, а действия не зависят от внешних факторов" />
            <LandingListItem title="Нет ограничений по числу тех, кто населяет метавселенную" />
            <LandingListItem title="В метавселенной своя экономика: люди получают «деньги» за проделанную «работу», владеют и распоряжаются имуществом" />
            <LandingListItem title="В метавселенной можно использовать элементы реального мира: например, работать на своем ноутбуке в виртуальном пространстве" />
            <LandingListItem title="Данные и цифровые активы из разных платформ совмещены: можно пользоваться вещами из Counter-Strike и Fortnite, покупать машину из Need for Speed и продавать ее друзьям на Facebook (принадлежит компании Meta, которая признана экстремисткой в России и запрещена)" />
            <LandingListItem title="Метавселенная наполнена «контентом и опытом», созданными ее пользователями, как отдельными людьми, так и организациями" />
          </ul>
        </div>
      </BaseSection>
    </section>

    <!-- Advanced trading tools section -->
    <section class="bg-trading-tools relative max-w-full sm:mx-4 my-20 py-16 shadow rounded-2xl overflow-hidden">
      <div class="relative max-w-screen-xl px-4 sm:px-2 mx-auto grid grid-cols-12 gap-x-6">
        <LandingTradingToolImage class="sm:hidden" />
        <div data-aos="fade-right" class="col-span-12 lg:col-span-6 space-y-8 sm:space-y-6 px-4 sm:px-6 mt-8">
          <h2 class="text-4xl font-semibold">Как будет выглядеть <span class="text-header-gradient">Метавселенная</span> в будущем?</h2>
          <div class="space-y-2">
            <h4 class="text-lg font-medium">Попробуем представить, как метаверсы будут выглядеть для обывателя в будущем, проведя прямые аналогии с сегодняшними технологиями.</h4>
            <p class="paragraph text-sm xl:text-base">
              Представим точку входа (устройство) в Метавселенную в виде компактных VR/AR очков. Их можно носить повседневно, цена в магазине приблизительно равна сегодняшним смартфонам.
            </p>
          </div>
          <div class="space-y-2">
            <p class="paragraph text-sm xl:text-base">
              Вы надеваете очки, включаете 1-2 кнопки, оказываетесь в виртуальной комнате и видите иконки приложений. Пространство очень похоже на рабочий стол в ОС Windows или окно смартфона.
            </p>
          </div>
          <div class="space-y-2">
            <p class="paragraph text-sm xl:text-base">
              Далее вы открываете браузер и вводите в адресную строку определенный сайт. Перед вами открывается портал (как из игры Portal), войдя в который начинается загрузка сайта/виртуального мира.
            </p>
          </div>
        </div>
        <LandingTradingToolImage data-aos="fade-left" class="hidden sm:block" />
      </div>
    </section>

    <!-- Getting started section -->
    <section class="bg-trading-tools relative max-w-full sm:mx-4 xl:mx-10 my-24 shadow sm:rounded-2xl overflow-hidden">
      <div class="w-full py-16 flex flex-col items-center">
        <h2 data-aos="flip-down" class="text-3xl sm:text-4xl font-semibold text-center">
          Мифы о <span class="text-header-gradient">Метавселенной</span>
        </h2>
        <div
          data-aos="fade-up"
          class="relative w-full flex flex-col lg:flex-row items-center justify-between space-y-12 lg:space-y-0 px-4 xl:px-10 mt-16 sm:mt-8"
        >
          <LandingStep v-for="step in steps" :key="step.title" :step="step" />
        </div>
      </div>
    </section>

    <div class="w-full my-10 flex justify-center">
      <a
        v-smooth-scroll
        data-aos="flip-down"
        data-aos-delay="150"
        href="#navbar"
        class="px-6 py-3 flex items-center space-x-2 bg-[#FAFAFA] hover:bg-gray-100 hover:shadow-md border border-[#DDDDDD] rounded-md text-gray-700"
      >
        <span>Back to top</span>
        <ArrowUpIcon :size="20" />
      </a>
    </div>
  </div>
</template>

<script>
import aosMixin from '@/mixins/aos'
export default {
  name: 'IndexPage',
  mixins: [aosMixin],
  data() {
    return {
      selected: 0,
      accordions: [
        {
          title: 'Why should I choose NEFA?',
          description:
            "We're industry pioneers, having been in the cryptocurrency industry since 2016. We've facilitated more than 21 billion USD worth of transactions on our exchange for customers in over 40 countries. Today, we're trusted by over 8 million customers around the world and have received praise for our easy-to-use app, secure wallet, and range of features.",
        },
        {
          title: 'How secure is NEFA?',
          description:
            "We're industry pioneers, having been in the cryptocurrency industry since 2016. We've facilitated more than 21 billion USD worth of transactions on our exchange for customers in over 40 countries. Today, we're trusted by over million customers around the world and have received praise for our easy-to-use app, secure wallet, and range of features.",
        },
        {
          title: 'Do I have to buy a whole Bitcoin?',
          description:
            "We're industry pioneers, having been in the cryptocurrency industry since 2016. We've facilitated more than 21 billion USD worth of transactions on our exchange for customers in over 40 countries. Today, we're trusted by over million customers around the world and have received praise for our easy-to-use app, secure wallet, and range of features.",
        },
        {
          title: 'How do I actually buy Bitcoin?',
          description:
            "We're industry pioneers, having been in the cryptocurrency industry since 2016. We've facilitated more than 21 billion USD worth of transactions on our exchange for customers in over 40 countries. Today, we're trusted by over million customers around the world and have received praise for our easy-to-use app, secure wallet, and range of features.",
        },
      ],
      steps: [
        {
          img: 'sign-up.png',
          title: 'Метавселенная – это игры с мультиплеером, где люди общаются и запускают мини-игры',
          description:
            'На данном этапе действительно популярны мета-пространства с мини-играми, вроде VRChat или Horizon Worlds. Но в будущем игры станут лишь опциональной функцией.',
        },
        {
          img: 'fund.png',
          title: 'Для входа обязательно нужен шлем виртуальной реальности',
          description:
            'В Roblox или Rec Room можно зайти со смартфона, а в VRChat с компьютера. А Decentraland вовсе не совместим с VR. Метаверс — не виртуальная реальность так же, как интернет – это не смартфон. VR-режим опционален.',
        },
        {
          img: 'buy-crypto.png',
          title: 'Это никому не нужно',
          description:
            '20 лет назад мало кто задумывался о том, насколько далеко зайдет Интернет. У метавселенной достаточно потенциала для того, чтобы стать следующей итерацией Интернета.\n' +
            '\n' +
            'Сейчас это выглядит как странный хайп: Nike делает цифровой магазин, Макдональдс – цифровое кафе, в котором можно заказать еду, и так далее.',
        },
      ],
    }
  },
}
</script>
<style scoped>

.text-header-gradient {
  background: rgb(57, 132, 244);
  background: linear-gradient(169.4deg, #3984f4 -6.01%, #0cd3ff 36.87%, #2f7cf0 78.04%, #0e65e8 103.77%);
  background-clip: text;
  -webkit-text-fill-color: transparent;
}
.bg-partner {
  background: rgb(57, 132, 244);
  background: linear-gradient(169.4deg, #3984f4 -6.01%, #0cd3ff 36.87%, #2f7cf0 78.04%, #0e65e8 103.77%);
  background-size: cover;
  background-position: center;
}
.bg-trading-tools {
  background: url('../assets/img/bg-trading-tools.webp');
  background-size: cover;
  background-position: center;
}
.max-h-0 {
  max-height: 0;
}
</style>
