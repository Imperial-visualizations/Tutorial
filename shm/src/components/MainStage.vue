<template>
    <div id="parent" style="height: 100%; width:50%">
        <canvas id="canvas"></canvas>
    </div>
</template>

<script>
export default {
    mounted(){
        let canvas = document.querySelector('canvas');
        let parent = document.getElementById('parent');

        canvas.width = parent.offsetWidth;
        canvas.height = parent.offsetHeight;
        
        let c = canvas.getContext('2d');

        function animate(){
            requestAnimationFrame(animate);

            c.clearRect(0,0,canvas.width, canvas.height);

            c.beginPath();
            c.arc(canvas.width/2, canvas.height/2, 50, 0, Math.PI * 2); 
            c.fillStyle = 'Orange';
            c.fill();
        }

        animate();
        

    }
    
}
</script>

<style>

</style>