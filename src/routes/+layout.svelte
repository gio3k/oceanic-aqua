<script>
    import "../app.css";
</script>

<style>
    .oca-background-container {
        position: fixed;
        z-index: -5;

        width: 100%;
        height: 100%;

        background-color: black;
    }

    .oca-background-item {
        position: absolute;

        width: 100%;
        height: 100%;
    }

    .oca-background-item.content {
        z-index: -4;

        object-fit: cover;

        transform: scale(1.5);
    }

    .oca-background-item.content video {
        width: 100%;
        height: 100%;

        object-fit: fill;
    }

    .oca-background-item.overlay {
        z-index: -3;

        -webkit-backdrop-filter: blur(70px);
        backdrop-filter: blur(70px);

        background-color: rgba(250, 250, 250, 0.7);
    }

    @media (prefers-color-scheme: light) {
        .oca-background-item.overlay {
            background-color: rgba(250, 250, 250, 0.7);
        }
    }

    @media (prefers-color-scheme: dark) {
        .oca-background-item.overlay {
            -webkit-backdrop-filter: blur(75px);
            backdrop-filter: blur(75px);
            background-color: rgba(30, 30, 30, 0.8);
        }
    }
</style>

<div class="oca-background-container">
    <div class="oca-background-item content">
        <video autoplay muted loop playsinline>
            <source src="backgrounds/videos/pb1.mp4" type="video/mp4"/>
        </video>
    </div>

    <div class="oca-background-item overlay">
    </div>
</div>

<slot/>