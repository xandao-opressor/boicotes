<template>
  <q-page class="index-page">
    <header class="top-header">
      <div class="inner">
        <div class="logo-wrapper q-pa-sm">
          <img src="/flag.svg" />
          <h1>Boicotes Brasil</h1>
        </div>
      </div>
    </header>

    <div class="row inner">
      <div class="col-xs-12 col-sm-7">
        <div class="q-pa-sm">
          <div class="flag">
            <h1>"Nossa bandeira jamais será vermelha!" - Brasileiros</h1>
            <div class="bg"></div>
          </div>
        </div>

        <section class="content-1 q-pa-sm">
          <div class="head socialism">
            <h2>Lula</h2>
            <p>Empresas que apoiam o socialismo/comunismo</p>
          </div>

          <q-list separator class="list-companies">
            <q-item v-for="(item, index) in communists" :key="index">
              <q-item-section avatar>
                <q-avatar size="xl">
                  <img class="logo" :src="item.src">
                </q-avatar>
              </q-item-section>
              <q-item-section>
                <q-item-label>
                  {{ item.company }}
                </q-item-label>
                <q-item-label caption>
                  {{  item.site }}
                </q-item-label>
              </q-item-section>
              <q-item-section side>
                <img src="/img/Foice.png" class="symbol" />
              </q-item-section>
            </q-item>
          </q-list>
        </section>

        <section class="content-1 q-pa-sm">
          <div class="head capitalism">
            <h2>Bolsonaro</h2>
            <p>Empresas que apoiam o Brasil</p>
          </div>

          <div class="list-companies">
            <q-list separator class="list-companies">
              <q-item v-for="(item, index) in capitalists" :key="index">
                <q-item-section avatar>
                  <q-avatar size="xl">
                    <img class="logo" :src="item.src">
                  </q-avatar>
                </q-item-section>
                <q-item-section>
                  <q-item-label>
                    {{ item.company }}
                  </q-item-label>
                  <q-item-label caption>
                    {{  item.site }}
                  </q-item-label>
                </q-item-section>
                <q-item-section side>
                  <img src="/img/Brazil.png" class="symbol" />
                </q-item-section>
              </q-item>
            </q-list>
          </div>
        </section>
      </div>
      <div class="col-xs-12 col-sm-5">
        <div class="about q-py-sm q-px-md">
          <h1 class="text-grey-9">Sobre</h1>

          <p>
            Assim como muitos brasileiros, que não se conforma com o rumo que ocorreu nas eleições e todos os seus fatos - evitar comentar detalhes pois não sabemos até onde vai à democracia, não é mesmo? 😌 - esta página foi criada.
          </p>

          <p>
            Por meio desta, devemos deixar de fácil acesso aos eleitores quais empresas apoiam o socialismo/comunismo (sim, o "novo" presidente <a href="https://noticias.r7.com/internacional/o-que-e-fato-sobre-as-relacoes-de-lula-e-do-pt-com-as-ditaduras-de-esquerda-13102022" target="_blank">apoia ditaduras</a>) e quais empresas não o fazem, que também manifestaram seu apoio ao Ex-Presidente Jair M. Bolsonaro ficando assim claro os seus valores.
          </p>

          <p>
            Em qualquer democracia (vamos acreditar que exista aqui), o boicote não é ilegal sendo aplicado em países livres e também como "arma" dos movimentos de esquerda contra instituições que não estejam alinhadas ao seu pensamento como o Sleeping Giants Brasil, por exemplo.
          </p>

          <p>
            Sinta-se à vontade para participar encaminhando em seus grupos, amigos, parentes, vizinhos, etc. Se por acaso existir divergência sobre o posicionamento da empresa, corrija-nos enviando um email para <a href="xandao_opressor@proton.me">xandao_opressor@proton.me</a> com à fonte da justificativa.
          </p>

          <p>
            Se você é desenvolvedor, pode realizar um <i>pull request</i> com melhorias/sugestões.
          </p>

          <p>
            Fique tranquilo, não vou lhe exigir 48h para justificar nada. 🫡
          </p>

          <p>
            <q-img src="/img/sociedade-ilustrada.jpg" />
          </p>
          <p>
            <a href="https://twitter.com/sigasociedade">
              <small>@sigasociedade</small>
            </a>
          </p>

        </div>
      </div>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'IndexPage',
  setup () {
    const capitalists = [
      {
        src: '/capitalism/BB.png',
        site: 'https://www.bb.com.br/',
        company: 'BB'
      },
      {
        src: '/capitalism/Beauty_in.png',
        site: 'https://www.beautyin.com/',
        company: 'Beauty\'in'
      },
      {
        src: '/capitalism/BioRitmo.png',
        site: 'https://www.bioritmo.com.br/',
        company: 'Academia Bio Ritmo'
      },
      {
        src: '/capitalism/BTGPactual.png',
        site: 'https://www.btgpactual.com/',
        company: 'BTG Pactual'
      },
      {
        src: '/capitalism/Centauro.png',
        site: 'https://www.centauro.com.br/',
        company: 'Centauro'
      },
      {
        src: '/capitalism/Cinemark.png',
        site: 'https://www.cinemark.com.br/',
        company: 'Cinemark'
      },
      {
        src: '/capitalism/CocoBambu.png',
        site: 'https://cocobambu.com/',
        company: 'Coco Bambu'
      },
      {
        src: '/capitalism/Cosan.png',
        site: 'https://www.cosan.com.br/',
        company: 'Cosan'
      },
      {
        src: '/capitalism/Drogaraia.png',
        site: 'https://www.drogaraia.com.br/',
        company: 'Droga Raia'
      },
      {
        src: '/capitalism/GazetaDoPovo.png',
        site: 'https://www.gazetadopovo.com.br/',
        company: 'Gazeta do Povo'
      },
      {
        src: '/capitalism/Gocil.png',
        site: 'https://gocil.com.br/',
        company: 'Gocil Segurança E Multisserviços'
      },
      {
        src: '/capitalism/Grendene.png',
        site: 'https://grendene.com.br/',
        company: 'Grendene'
      },
      {
        src: '/capitalism/Habibs.png',
        site: 'https://www.habibs.com.br/',
        company: 'Habib\'s'
      },
      {
        src: '/capitalism/Havan.png',
        site: 'https://www.havan.com.br/',
        company: 'Havan'
      },
      {
        src: '/capitalism/Jeronimo.png',
        site: 'https://jeronimoburger.com.br/',
        company: 'Jeronimo Burger'
      },
      {
        src: '/capitalism/LivrariaCultura.png',
        site: 'https://www.livrariacultura.com.br/',
        company: 'Livraria Cultura'
      },
      {
        src: '/capitalism/Localiza.png',
        site: 'https://www.localiza.com/brasil/',
        company: 'Localiza'
      },
      {
        src: '/capitalism/Madero.png',
        site: 'https://www.restaurantemadero.com.br/',
        company: 'Madero'
      },
      {
        src: '/capitalism/Marabraz.png',
        site: 'https://www.marabraz.com.br/',
        company: 'Marabraz'
      },
      {
        src: '/capitalism/Marisa.png',
        site: 'https://www.marisa.com.br/',
        company: 'Marisa'
      },
      {
        src: '/capitalism/Marisol.png',
        site: 'https://www.clubemarisol.com.br/',
        company: 'Marisol'
      },
      {
        src: '/capitalism/Mormaii.png',
        site: 'https://www.mormaiishop.com.br/',
        company: 'Mormaii'
      },
      {
        src: '/capitalism/Multiplan.png',
        site: 'https://www.multiplan.com.br/',
        company: 'Multiplan'
      },
      {
        src: '/capitalism/MundoVerde.png',
        site: 'https://www.mundoverde.com.br/',
        company: 'Mundo Verde'
      },
      {
        src: '/capitalism/OticasCarol.png',
        site: 'https://www.oticascarol.com.br/brasil',
        company: 'Óticas Carol'
      },
      {
        src: '/capitalism/PizzaHut.png',
        site: 'https://www.pizzahut.com.br/',
        company: 'Pizza Hut'
      },
      {
        src: '/capitalism/Polishop.png',
        site: 'https://www.polishop.com.br/',
        company: 'Polishop'
      },
      {
        src: '/capitalism/Purina.png',
        site: 'https://purina.com.br/',
        company: 'Purina'
      },
      {
        src: '/capitalism/Ragazzo.png',
        site: 'https://www.deliveryragazzo.com.br/',
        company: 'Ragazzo!'
      },
      {
        src: '/capitalism/Riachuelo.png',
        site: 'https://www.riachuelo.com.br/',
        company: 'Lojas Riachuelo'
      },
      {
        src: '/capitalism/Smartfit.png',
        site: 'https://www.smartfit.com.br/',
        company: 'Smart Fit'
      },
      {
        src: '/capitalism/Tecnisa.png',
        site: 'https://www.tecnisa.com.br/',
        company: 'Tecnisa'
      },
      {
        src: '/capitalism/Topper.png',
        site: 'https://www.topper.com.br/',
        company: 'Topper'
      },
      {
        src: '/capitalism/Ype.png',
        site: 'https://www.ype.ind.br',
        company: 'Ype'
      },
      {
        src: '/capitalism/Zara.png',
        site: 'https://www.zara.com/',
        company: 'Zara Brasil'
      }
    ]

    const communists = [
      {
        src: '/communist/Ambev.png',
        site: 'https://www.ambev.com.br/',
        company: 'Ambev'
      },
      {
        src: '/communist/Americanas.png',
        site: 'https://www.americanas.com.br/',
        company: 'Americanas'
      },
      {
        src: '/communist/Bayer.png',
        site: 'https://www.americanas.com.br/',
        company: 'Bayer'
      },
      {
        src: '/communist/Boticario.png',
        site: 'https://www.boticario.com.br/',
        company: 'Boticário'
      },
      {
        src: '/communist/Bradesco.png',
        site: 'https://www.bradesco.com.br/',
        company: 'Bradesco'
      },
      {
        src: '/communist/braskem.png',
        site: 'https://www.braskem.com.br/',
        company: 'Braskem'
      },
      {
        src: '/communist/BurgerKing.png',
        site: 'https://www.burgerking.com.br/',
        company: 'Burger King'
      },
      {
        src: '/communist/Boticario.png',
        site: 'https://www.boticario.com.br/',
        company: 'Boticário'
      },
      {
        src: '/communist/Carrefour.png',
        site: 'https://www.carrefour.com.br/',
        company: 'Carrefour'
      },
      {
        src: '/communist/Danone.png',
        site: 'https://www.danone.com.br/',
        company: 'Danone'
      },
      {
        src: '/communist/Folha.png',
        site: 'https://www.folha.uol.com.br/',
        company: 'Folha de São Paulo'
      },
      {
        src: '/communist/Friboi.png',
        site: 'https://www.friboi.com.br/',
        company: 'Friboi'
      },
      {
        src: '/communist/Itau.png',
        site: 'https://www.itau.com.br/',
        company: 'Itaú'
      },
      {
        src: '/communist/Klabin.png',
        site: 'https://www.klabin.com.br/',
        company: 'Klabin'
      },
      {
        src: '/communist/LOccitane.png',
        site: 'https://br.loccitane.com/',
        company: 'L\'Occitane'
      },
      {
        src: '/communist/Magalu.png',
        site: 'https://www.magalu.com.br/',
        company: 'Magalu'
      },
      {
        src: '/communist/natura.png',
        site: 'https://www.natura.com.br/',
        company: 'Natura'
      },
      {
        src: '/communist/Nestle.png',
        site: 'https://www.nestle.com.br/',
        company: 'Nestlé'
      },
      {
        src: '/communist/Popeyes.png',
        site: 'https://www.popeyesbrasil.com.br/',
        company: 'Popeyes Brasil'
      },
      {
        src: '/communist/PostoIpiranga.png',
        site: 'https://www.portal.ipiranga/',
        company: 'Posto Ipiranga'
      },
      {
        src: '/communist/Santander.png',
        site: 'https://www.santander.com.br/',
        company: 'Santander'
      },
      {
        src: '/communist/Submarino.png',
        site: 'https://www.submarino.com.br/',
        company: 'Submarino'
      },
      {
        src: '/communist/Suzano.png',
        site: 'https://www.klabin.com.br/',
        company: 'Suzano Papel e Celulose'
      },
      {
        src: '/communist/Tecmundo.png',
        site: 'https://www.tecmundo.com.br/',
        company: 'Tecmundo'
      },
      {
        src: '/communist/ultragaz.png',
        site: 'https://www.ultragaz.com.br/',
        company: 'Ultragaz'
      }
    ]

    return {
      capitalists,
      communists
    }
  }
})
</script>
