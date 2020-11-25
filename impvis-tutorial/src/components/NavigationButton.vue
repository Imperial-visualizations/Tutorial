<template>
    <div>
        <div class="nav-group">
            <iv-button class="nav-button">
                <a
                    :href="'./' + 'page_' + (pageNumber - 1) + '.html'"
                    class="nav-button-text"
                    >previous</a
                >
            </iv-button>
            <iv-button class="nav-button">
                <a
                    :href="'./' + 'page_' + (pageNumber + 1) + '.html'"
                    class="nav-button-text"
                    >next</a
                >
            </iv-button>
            <iv-pane-navigator />
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
            console.log("pageName", this.pageName);
            return Number(this.pageName.slice(4));
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
    margin-right: 20px;
    margin-bottom: 20px;
    background: #133f6f;
}
.nav-button-text {
    color: white;
}
</style>
