<template>
    <div id="parent" style="height: 50%; width:50%; padding:50px;">
        <canvas id="canvas"></canvas>
    </div>
</template>

<script>
export default {
    props:{
        freq: {
            default: 0.005,
        },
        amp: {
            default: 50,
        }
    },
    mounted(){
        let vm = this;
        let canvas = document.querySelector('canvas');
        let parent = document.getElementById('parent');
        canvas.width = parent.offsetWidth;
        canvas.height = parent.offsetHeight;
        let c = canvas.getContext('2d');

        let amp = vm.amp;
        let freq = vm.freq;
        let x = amp + canvas.width/2;
        let dx = 0;

        function animate(){
            requestAnimationFrame(animate);

            //Check for prop changes
            if(amp !== vm.amp || freq !== vm.freq){
                amp = vm.amp;
                freq = vm.freq;
                console.log('value change');
                x = amp + canvas.width/2;
                dx = 0;
            }
        

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
            dx += - freq * (x-canvas.width/2);
        }

        animate();
        
        

    }
    
}
</script>

<style>

</style>