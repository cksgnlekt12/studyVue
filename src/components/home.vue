
<template>
<!-- template side는 일반적인 html 문법을 사용 -->
  <!-- 클래스 바인딩 -->
  <div class="classBinding" :class="{test:true, activate:isActive}">Hello World1111</div>

  <!-- 스타일 바인딩 -->
  <div :style="{color: colorRed}">Hello World2222</div>

  <!-- 데이터 바인딩 -->
  <div :class="{test:isActive}">{{isActive}}</div>

  <!-- 조건문 -->
  <div v-if="ifTest">If문 테스트중.</div>
  <div v-else-if="ifTest2">If문2 테스트중.</div>
  <div v-else>else문 테스트중.</div>
  <div v-show="false">show문</div>

  <!-- 반복문 -->
  <div v-for="(i,no) in is" :key="i*2">for문 테스트 {{i}}/{{is}} ({{no}})</div>
  <!-- 이벤트 바인딩 -->
  <div class="eventBinding">{{testLog()}}
    <div v-on:click="testLog()">이벤트 바인딩 (클릭하면 로그)</div>
    <div @click="testLog()">이벤트 바인딩@방식 (클릭하면 로그)</div>
  </div>

  <!-- 양방향 바인딩 -->
  <div>
    <!-- input 태그로 v-model 에서 데이터 바인딩의 보간없이 작성하여 미리 입력된 예제. -->
    <input v-model="message" placeholder="입력" />
    <p>메시지: {{ message }}</p>
    <input type="button" value="초기화" @click="message='초기화'">
  </div>

  <!-- methods, computed, watch 테스트 -->
  <div class="sub">
      methods - count: {{methodsCount()}}<br>
      <input type="button" value="증가" @click="countMethods++">
      <input type="button" value="감소" @click="countMethods--"><br>
      computed - count: {{computedCount}}<br>
      <input type="button" value="증가" @click="countComputed++">
      <input type="button" value="감소" @click="countComputed--"><br>
  </div>
</template>

<script>
// script side는 내부에서 이루어지는 데이터를 관리.
export default {
  data(){
    return{
      isActive : true,
      a : 'test',
      colorRed: '#ff0000',
      message: '테스트',
      ifTest: false,
      ifTest2: true,
      is: 5,
      no: 1,
      countMethods: 0,
      countComputed: 0
    }
  },
  methods: {
    testLog (){
      console.log('methods 테스트');
      return this.message;
    },
    methodsCount(){
      console.log('methods!');
      // return this.countMethods;
    }
  },
  computed: {
    computedCount() {
      console.log('computed');
      return this.countComputed;
    }
  },
  watch: {
    // 이쪽은 data의 이름과 일치해야 함(?)
    // message(){
    //   console.log('watch Test')
    // }
  },
  /* methods, compute, watch 차이점.
  methods : template 내의 어떤 것이든 변경되면 작동
  computed : template 내의 값 중 함수와 연결된 값이 바뀔때 작동
  watch : template 내의 값이 지정된 변수가 값만 변경됐다 하면 작동
  */
  name: 'home',
  props: {
    msg: String
  }
}
</script>

<!-- scoped 속성 추가시 해당 컴포넌트에서만 적용되는 Style 지정. -->
<style scoped>
div {
  font-size: 20px;
  line-height: 30px;
}
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
