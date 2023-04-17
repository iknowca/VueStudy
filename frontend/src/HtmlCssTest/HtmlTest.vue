<template>
<div>
    <h3>
        실제 코드 형태로 입력해보기
    </h3>
    <h6>원래 코드 형태 출력이 아닌 실제 코드가 동작해야 함.</h6>
    <h4>chatGPT같은 걸 만든다면 필요할 수도?</h4>

    <pre style="text-align: left;">
        function saveLocalData () {
                let second = document.getElementById("second")
                let value = second.value
                localStorage.setItem(1, value)
                getLocalData()
            }
    </pre>
</div>
</template>

<script>
export default {
    name: "HtmlTest"
}
</script>

<style scoped>

</style>