# GreatPages-Background-Video

<a href="https://www.buymeacoffee.com/claitonllemes" target="_blank" rel="noopener noreferrer"><img src="https://user-images.githubusercontent.com/99222756/210368404-216273fb-c930-453e-b32b-e3614872eba3.png" width="100%"/></a><br>

## **Configurações**
O código abaixo adiciona um vídeo ao fundo de um bloco na plataforma Greatpages. Copie e cole no menu de configurações da página.

<br><a href="https://www.buymeacoffee.com/claitonllemes" target="_blank" rel="noopener noreferrer"><img src="https://user-images.githubusercontent.com/99222756/210372197-a1d41894-8acc-470b-ac38-2bd1ee0a4ed9.png" width="100%"/></a><br>


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