<template>
  <div class="clearAllContainer">
  	<span class="clearAllBtn" @click="clearTodo">Clear All</span>
  </div>
</template>

<script>
export default {
	methods: {
		clearTodo() {
			// 로컬스토리지의 데이터 모두 삭제
			localStorage.clear();
		}
	}
}
</script>

<style scoped>
.clearAllContainer {
	width: 8.5rem;
	height: 50px;
	line-height: 50px;
	background: #fff;
	border-radius: 5px;
	margin: 0 auto;
}
.clearAllBtn {
	display: block;
	color: #e20303;
}
</style>