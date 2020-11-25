<template>
    <div class="nav-group">
        <a
            :href="'./' + 'page_' + (pageNumber - 1) + '.html'"
            class="iv-button nav-button nav-button-text"
            >Previous</a
        >
        <a
            :href="'./' + 'page_' + (pageNumber + 1) + '.html'"
            class="iv-button nav-button nav-button-text"
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
    },
};
</script>
<style>
.nav-group {
    position: relative;
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: flex-end;
}
.nav-button {
    display: block;
    width: 4.8rem;
    margin-right: 1.5rem;
    margin-bottom: 2rem;
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
