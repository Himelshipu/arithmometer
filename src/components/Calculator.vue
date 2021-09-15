<template>
  <!-- calculator -->
  <div class="mx-auto overflow-hidden mt-10 shadow-lg mb-2 bg-gray-300 shadow-lg border rounded-lg lg:w-2/6 md:w-3/6 sm:w-4/6">

    <div class="">

      <div class="p-5 text-white text-center text-3xl bg-blue-500">

<!--    <img alt="Vue logo" src="/src/assets/favicon.png" class="mx-auto h-12"> -->

        <span class=" uppercase">Arithmometer</span></div>

      <div class="pt-16 p-5 pb-0 text-blue-500 text-right text-3xl bg-gray-200"> {{current || 0}} </div>

<!-- <div class="p-5 text-white text-right text-3xl bg-blue-500">= <span class="text-orange-500">2100</span></div> -->

      <div class="flex items-stretch  h-24">

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold ">
          <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none" @click="percent" >%</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none" @click="sign">+/-</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div class="rounded-full h-20 w-20 flex items-center bg-red-500 justify-center shadow-lg border-2 border-red-500 hover:border-2 hover:border-white focus:outline-none"  @click="clear">C</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div class="rounded-full h-20 w-20 flex items-center bg-red-500 justify-center shadow-lg border-2 border-red-500 hover:border-2 hover:border-white focus:outline-none">CE</div>
        </div>
      </div>

      <div class="flex items-stretch  h-24">
        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none" @click="append('7')">7</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none" @click="append('8')">8</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none" @click="append('9')">9</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none"  @click="divide">÷</div>
        </div>
      </div>

      <div class="flex items-stretch  h-24">
        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none" @click="append('4')">4</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none" @click="append('5')">5</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none" @click="append('6')">6</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none"  @click="multiply">×</div>
        </div>
      </div>

      <div class="flex items-stretch  h-24">
        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none" @click="append('1')">1</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none" @click="append('2')">2</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none" @click="append('3')">3</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none"  @click="plus">+</div>
        </div>
      </div>

      <div class="flex items-stretch h-24 mb-4">

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none" @click="append('0')">0</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none" @click="dot">.</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none" @click="equal">=</div>
        </div>

        <div class="flex-1 px-2 py-2 justify-center flex items-center text-white text-2xl font-semibold">
          <div class="rounded-full h-20 w-20 flex items-center bg-blue-500 justify-center shadow-lg border-2 border-blue-500 hover:border-2 hover:border-white focus:outline-none"  @click="minus">-</div>
        </div>


      </div>

    </div>
  </div>
</template>

<script>
export default {
  data(){
    return {
      current :'',
      previous : null,
      operator:null,
      operatorClicked : false
    }
  },
  methods:{
  clear(){
    this.current =''
  },
    sign(){
    this.current = this.current.charAt(0) === '-' ?
        this.current.slice(1) : `-${this.current}`
    },
    percent(){
    this.current = `${parseFloat(this.current)/100}`
    },
    append(number){
      if(this.operatorClicked){
        this.current ='';
        this.operatorClicked =false;
      }
      this.current =`${this.current}${number}`;
    },
    dot(){
    if (this.current.indexOf('.') === -1){
        this.append('.');
    }
    },
    setPrevious(){
      this.previous = this.current;
      this.operatorClicked = true;
    },
    divide(){
    this.operator = (a,b)=> a/b;
    this.setPrevious();
    },
    multiply(){
    this.operator = (a,b)=> a*b;
    this.setPrevious();
    },
    plus(){
    this.operator = (a,b)=> a*b;
    this.setPrevious();
    },
    minus(){
    this.operator = (a,b)=> a-b;
    this.setPrevious();
    },
    equal(){
    this.current = `${this.operator(
    parseFloat(this.current),
    parseFloat(this.previous)
      )}` ;
    this.previous = null;

    },
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
