<template>
    <li id="ttl" class="list-group-item d-flex">
        <div id="ttltext">
        {{ t.title }}
        </div>
        <div id="per">
        {{ t.percent }}%
        <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" fill="currentColor" class="bi bi-record-fill" viewBox="0 0 16 16">
        <path fill-rule="evenodd" d="M8 13A5 5 0 1 0 8 3a5 5 0 0 0 0 10z"/>
        </svg>
        </div>
        <button type="button" class="btn btn-outline-dark">Подробнее</button>
    </li>
</template>

<script>
export default {
    props: {
        t: {
            type: Object,
            required: true
        }
    }
}
</script>

<style scoped>
#ttl {
    width: 50%;
    height: 60px;
}
.li {
    display: flex;
    justify-content: space-between;
    padding: 10px;
}
#per {
    align-items: center;
    display: flex;
    padding-right: 0px;
    padding-left: 50%;
    color: red;
}
#ttltext {
    width: 50%;
    margin-left: 0px;
}

</style>
