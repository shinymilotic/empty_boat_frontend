<script lang="ts">
    let src: string = "https://assets.nintendo.com/image/upload/ar_16:9,c_lpad,w_656/b_white/f_auto/q_auto/store/software/switch/70010000000025/7137262b5a64d921e193653f8aa0b722925abc5680380ca0e18a5cfd91697f58";
    let name: string = "Zelda: The Legend of Zelda";
    let alt: string = "Game name: " + name;
</script>

<img src="{src}" alt="Zelda" />

<img {src} alt="Game name: {name}" />

<img {src} {alt} />