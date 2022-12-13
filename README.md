# GreatPages-Background-Video

#### Adiciona Vídeo ao fundo de um bloco na plataforma GreatPages

<br>

<img src="https://user-images.githubusercontent.com/99222756/207317647-1c517d05-a17f-4f25-bbf5-33cbb236e85e.jpg" width="100%"/>

<br>


```html

<script>
    $('#ID_BLOCO').append(
        '<video autoplay="" muted="" loop="" playsinline="" id="vid" preload="auto" width="100%" height="100%" volume="0" canplay="false"><source src="URL_DO_VÍDEO" type="video/mp4"></video><div class="overlay"></div>');
</script>

<style>
    video {
        filter: grayscale(100%);
        position: absolute;
        top: 0;
        left: 0;
        display: block;
        width: 100%;
        height: 100%;
        object-fit: cover;
        z-index: 0;
    }

    .overlay {
        width: 100%;
        height: 100%;
        position: absolute;
        top: 0;
        left: 0;
        background-image: linear-gradient(45deg, rgba(0, 0, 0, .1) -30%, rgba(0, 0, 0, 1) 80%);
        background-size: 3px 3px;
        z-index: 1;
    }
</style>

```