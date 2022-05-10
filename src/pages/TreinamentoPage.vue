<template>
  <q-page class="row flex-center bg-grey-12">
    <div class="col-md-5 col-xs-12 q-pa-md">
      <div class="row">
        <q-input class="full-width" outlined></q-input>
      </div>
      <div class="row q-mt-sm">
        <div class="col">
          <q-btn
            class="full-width"
            size="lg"
            color="secondary"
            label="AC"
          ></q-btn>
        </div>
        <div class="col">
          <q-btn
            class="full-width"
            size="lg"
            color="secondary"
            label="-/+"
          ></q-btn>
        </div>
        <div class="col">
          <q-btn
            class="full-width"
            size="lg"
            color="secondary"
            label="%"
          ></q-btn>
        </div>
        <div class="col">
          <q-btn class="full-width" size="lg" color="accent" label="/"></q-btn>
        </div>
      </div>
      <div class="row">
        <div class="col">
          <q-btn
            class="full-width"
            size="lg"
            color="secondary"
            label="7"
          ></q-btn>
        </div>
        <div class="col">
          <q-btn
            class="full-width"
            size="lg"
            color="secondary"
            label="8"
          ></q-btn>
        </div>
        <div class="col">
          <q-btn
            class="full-width"
            size="lg"
            color="secondary"
            label="9"
          ></q-btn>
        </div>
        <div class="col">
          <q-btn class="full-width" size="lg" color="accent" label="X"></q-btn>
        </div>
      </div>
      <div class="row">
        <div class="col">
          <q-btn
            class="full-width"
            size="lg"
            color="secondary"
            label="4"
          ></q-btn>
        </div>
        <div class="col">
          <q-btn
            class="full-width"
            size="lg"
            color="secondary"
            label="5"
          ></q-btn>
        </div>
        <div class="col">
          <q-btn
            class="full-width"
            size="lg"
            color="secondary"
            label="6"
          ></q-btn>
        </div>
        <div class="col">
          <q-btn class="full-width" size="lg" color="accent" label="-"></q-btn>
        </div>
      </div>
      <div class="row">
        <div class="col">
          <q-btn
            class="full-width"
            size="lg"
            color="secondary"
            label="1"
          ></q-btn>
        </div>
        <div class="col">
          <q-btn
            class="full-width"
            size="lg"
            color="secondary"
            label="2"
          ></q-btn>
        </div>
        <div class="col">
          <q-btn
            class="full-width"
            size="lg"
            color="secondary"
            label="3"
          ></q-btn>
        </div>
        <div class="col">
          <q-btn class="full-width" size="lg" color="accent" label="+"></q-btn>
        </div>
      </div>
      <div class="row">
        <div class="col">
          <q-btn
            class="full-width"
            size="lg"
            color="secondary"
            label="0"
          ></q-btn>
        </div>
        <div class="col">
          <q-btn
            class="full-width"
            size="lg"
            color="secondary"
            label="0"
          ></q-btn>
        </div>
        <div class="col">
          <q-btn
            class="full-width"
            size="lg"
            color="secondary"
            label="."
          ></q-btn>
        </div>
        <div class="col">
          <q-btn class="full-width" size="lg" color="accent" label="="></q-btn>
        </div>
      </div>
    </div>
  </q-page>
</template>

<script>
import { defineComponent, ref } from "@vue/runtime-core";

export default defineComponent({
  name: "TreinamentoPage",

  setup() {
    //// Declara as variaveis
    //// Variavais servem para armazenar os dados

    //var minhavariavel = "teste";
    //const minhavariavel = ref(null);
    //const minhavariavel = "teste";
    //let minhavariavel = "teste";

    // Tipos de dados para colocar dentro das variaveis
    var Tantofaznumero1 = 7;
    var Tantofaznumero2 = 9.5;
    var Tantofaztexto = "9";
    var Tantofazbooleano = false;
    //console.log(Tantofazbooleano);
    var TantofazArray1 = [1, 2, 3];
    var TantofazArray2 = ["texto1", "4", "x"];
    var TantofazArray3 = [true, false, true, false];

    var total = 0;

    var TantofazObject = {
      nome: "teste",
      idade: 1,
      qualidades: ["feio", "bonito"],
    };

    //console.log(total);
    total = total + 5;
    total = total + 8;
    //console.log(total);

    let teste5 = 5; // criada fora do metodo

    const minhavariavel = ref(null);
    // Cria o metodo
    const metodoTeste1 = () => {
      const banana = "banana ";
      //console.log(banana);
      minhavariavel.value = banana;
    };
    // // Cria o metodo
    const metodoTeste2 = () => {
      const banana = "é uma fruta ";
      //console.log(banana);
      minhavariavel.value = minhavariavel.value + banana;
    };
    // // Cria o metodo
    const metodoTeste3 = () => {
      const banana = 8;
      //console.log(banana);
      minhavariavel.value = minhavariavel.value + banana;
    };
    // // Chama ou aciona o metodo
    const metodoTeste4 = () => {
      metodoTeste1();
      metodoTeste2();
      metodoTeste3();
    };

    // Operadores aritmeticos
    const metodoSoma = () => {
      const a = 5;
      const b = 3;
      const soma = a + b;
      return soma;
    };

    const metodoTesteOperadores = () => {
      const numero1 = 9;
      const numero2 = 7;
      const total = numero1 + numero2 + metodoSoma() + 2;
      console.log(total);

      const texto1 = "teste1";
      const texto2 = "teste2";
      console.log(texto1 + " " + texto2);
    };

    //Operadores logicos e condicionais
    const metodoOperaoresCondicionais_IF = () => {
      const operador = "-";
      const compra = 1;
      const condicao = true;

      if (condicao == false) {
        console.log("Operador +");
      } else {
        console.log("Operador verdadeiro");
      }

      if (operador == "-") {
        console.log("Operador -");
      }

      if (operador == "/") {
        console.log("Operador /");
      }
      //console.log("Chegou aqui");
    };
    //Looping
    const metodoOperaoresCondicionais_FOR = () => {
      //let contador = 10;
      let mercado = "leite";

      //Inicio do loop // Ate que isso aconteça // Incremento
      for (let contador = 0; contador < 10; contador++) {
        console.log("Chegou aqui " + contador);

        if (contador == 5) {
          console.log("Garrafa de leite");
        }
        //metodoTesteOperadores();
      }
    };

    metodoOperaoresCondicionais_FOR();
    console.log("Chegou aqui");

    return {
      total,
      minhavariavel,
      metodoTeste4,
    };
  },
});
</script>

<style>
.fundo-verde {
  background-color: #00ff00;
}
</style>
