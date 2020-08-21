<template>
    <div id="parent" style="height: 50%; width:50%; padding:50px;">
        <canvas id="canvas"></canvas>
    </div>
</template>

<script>
export default {
    props:{
        mag: {
            default: 0.005,
        }
    },
    mounted(){
        let vm = this;
        let canvas = document.querySelector('canvas');
        let parent = document.getElementById('parent');
        let x = 50 + canvas.width/2;
        let dx = 0;

        canvas.width = parent.offsetWidth;
        canvas.height = parent.offsetHeight;
        
        let c = canvas.getContext('2d');

        function animate(){
            requestAnimationFrame(animate);

            c.clearRect(0,0,canvas.width, canvas.height);

            c.beginPath();
            c.moveTo(0,0);
            c.lineTo(canvas.width, 0);
            c.lineTo(canvas.width, canvas.height);
            c.lineTo(0, canvas.height);
            c.lineTo(0, 0);
            c.strokeStyle = 'black';
            c.stroke();

            c.beginPath();
            c.moveTo(x, canvas.height/2);
            c.lineTo(canvas.width/2, canvas.height/2);
            c.strokeStyle = 'blue';
            c.lineWidth = 2;
            c.stroke();

            c.beginPath();
            c.arc(x, canvas.height/2, 20, 0, Math.PI * 2); 
            c.fillStyle = 'orange';
            c.fill();

            x += dx;
            dx += - vm.mag * (x-canvas.width/2);
        }

        animate();
        

    }
    
}
</script>

<style>

</style>