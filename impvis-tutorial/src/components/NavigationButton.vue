<template>
    <div class="nav-group">
        <a
            :href="'./' + 'page_' + (pageNumber - 1) + '.html'"
            class="iv-button nav-button nav-button-text"
            v-if="shouldRenderPrevious"
            >Previous</a
        >
        <a
            :href="'./index.html'"
            class="iv-button nav-button nav-button-text"
            >Contents</a
        >
        <a
            :href="'./' + 'page_' + (pageNumber + 1) + '.html'"
            class="iv-button nav-button nav-button-text"
            v-if="shouldRenderNext"
            >Next</a
        >
    </div>
</template>

<script>
export default {
    props: {
        pageName: {
            type: String,
            required: true,
        },
    },
    computed: {
        pageNumber: function() {
            let num = Number(this.pageName.slice(4));
            console.log("pageName", num);
            return num;
        },
        shouldRenderPrevious: function() {
            return this.pageNumber - 1 >= 1
        },
        shouldRenderNext: function() {
            return this.pageNumber + 1 <= 50
        }
    },
};
</script>
<style>
.nav-group {
    position: relative;
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: center;
}
.nav-button {
    display: block;
    width: 4.8rem;
    margin-right: 1rem;
    margin-left: 1rem;
    margin-bottom: 1rem;
    margin-top: 2rem;
    background: #133f6f;
}
.nav-button:hover {
    background:#3e668b
}
.nav-button-text {
    color: white;
    text-decoration: none;
}
</style>
