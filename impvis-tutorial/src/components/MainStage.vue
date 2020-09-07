<template>
    
</template>

<script>
export default {
    props:{
        mag: {
            default: 0.005,
        }
    },
    mounted(){
        //let vm = this;
        let canvas = document.querySelector('cancas');
        let parent = document.getElementById('parent');
        //let x = 50 +canvas.width/2;
        //let dx = 0;

        canvas.width = parent.offsetWidth;
        canvas.height = parent.offsetHeight;

        let c = canvas.getContext('2d');

        function animate(){
            requestAnimationFrame(animate);

            c.clearRect(0,0,canvas.width, canvas, canvas.height);

            c.beginPath();
            c.moveTo(0,0);
            c.lineTo(canvas.width, 0);
            c.lineTo(canvas.width, canvas.height);
            c.lineTo(0, canvas.height);
            c.lineTo(0,0);
            c.strokeStyle - 'black';
            c.stroke();
        }
        
        animate();
    }
}
</script>

<style>

</style>