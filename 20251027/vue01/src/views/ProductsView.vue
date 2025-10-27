<template>
    <div>
        <h2>상품 페이지</h2>
        <p>장 바구니에 담긴 상품 수 : {{counter.count}}</p>
        <button @click="counter.increment">상품 추가</button>
        <button @click="counter.rest">리셋</button>
    </div>
</template>

<script setup>
import {useCounterStore} from '../stores/counter'
const counter = useCounterStore()
</script>