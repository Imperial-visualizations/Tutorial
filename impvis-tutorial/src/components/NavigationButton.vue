<template>
    <div>
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
            console.log("pageName", this.pageName.slice(5));
            return Number(this.pageName.slice(5));
        },
    },
};
</script>
<style>
.nav-group {
    position: absolute;
    bottom: 0px;
    right: 0px;
}
.nav-button {
    width: 4.8rem;
    margin-right: 20px;
    margin-bottom: 20px;
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
