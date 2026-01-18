# FOR-Gree-
</html><!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Para Gree 🌻</title>

<style>
body {
    margin: 0;
    height: 100vh;
    background: #fde2eb;
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: 'Segoe UI', sans-serif;
}

/* ===== LAYOUT GENERAL ===== */
.layout {
    display: flex;
    align-items: center;
    gap: 25px;
}

/* ===== IMÁGENES LATERALES ===== */
.side-img {
    width: 110px; /* puedes subir a 130 si quieres */
    opacity: 0.95;
}

/* ===== TARJETA ===== */
.card {
    width: 330px;
    height: 480px;
    background: white;
    border-radius: 30px;
    box-shadow: 0 15px 40px rgba(0,0,0,0.15);
    overflow: hidden;
    position: relative;
}

/* ===== PORTADA ===== */
.cover {
    position: absolute;
    inset: 0;
    background: linear-gradient(180deg, #f8c8dc, #fff);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    transition: transform 0.8s ease;
    z-index: 2;
}

.cover img {
    width: 180px;
    margin-bottom: 20px;
}

.cover h1 {
    font-size: 22px;
    color: #444;
    margin: 0;
}

.cover p {
    font-size: 14px;
    color: #777;
    margin: 8px 0 20px;
}

.btn {
    padding: 10px 22px;
    border-radius: 20px;
    border: none;
    background: #e0a800;
    color: white;
    font-size: 14px;
    cursor: pointer;
}

/* ===== CONTENIDO ===== */
.content {
    padding: 30px 25px;
    text-align: center;
}

.sunflower {
    font-size: 60px;
    margin-bottom: 10px;
}

.text {
    font-size: 15px;
    color: #444;
    line-height: 1.6;
}

.highlight {
    color: #f2a1c7;
    font-weight: 600;
}

.signature {
    margin-top: 18px;
    font-size: 14px;
    color: #777;
}

/* ===== ANIMACIÓN ===== */
.open {
    transform: translateY(-100%);
}
</style>
</head>

<body>

<!-- ===== MÚSICA ===== -->
<audio id="music" loop>
    <source src="https://image2url.com/r2/default/audio/1768771784857-5ea5d26d-718f-48f1-b8b9-e8a0792ad31a.mp3" type="audio/mpeg">
</audio>

<script>
document.addEventListener("click", function playMusicOnce() {
    const music = document.getElementById("music");
    music.volume = 0.4;
    music.play();
    document.removeEventListener("click", playMusicOnce);
});

function openCard() {
    document.getElementById('cover').classList.add('open');
}
</script>

<!-- ===== ESTRUCTURA CORRECTA ===== -->
<div class="layout">

    <!-- IMAGEN IZQUIERDA -->
    <img src="https://image2url.com/r2/default/images/1768777641389-a11f6cd6-ec32-4b77-91bd-bc3e70979bd2.jpeg" class="side-img">

    <!-- TARJETA -->
    <div class="card">

        <!-- PORTADA -->
        <div class="cover" id="cover">
            <img src="https://image2url.com/r2/default/images/1768769393289-d615c39e-93ba-43b9-be36-b9b30a41d047.png">
            <h1>Toca aquí 🌻</h1>
            <p>Cuando estés lista</p>
            <button class="btn" onclick="openCard()">Abrir</button>
        </div>

        <!-- CONTENIDO -->
        <div class="content">
            <div class="sunflower">🌻</div>

            <div class="text">
                Me gustó verte, reírnos<br>
                y compartir contigo lo que nunca he hecho.<br><br>

                Gracias por el osito con tu perfume y el Hot Wheels,<br>
                mirarte y acariciarte se siente único.<br>
                Aunque cometa errores, quiero mejorar<br>
                para no dañar tu corazoncito.<br><br>

                No creí sentir esto que siento por ti,<br>
                tú eres <span class="highlight">algo bonito</span><br>
                que quiero cuidar.
            </div>

            <div class="signature">
                — Para ti, Gree 🌻
            </div>
        </div>

    </div>

    <!-- IMAGEN DERECHA -->
    <img src="https://image2url.com/r2/default/images/1768777671546-6df4e8e5-ab43-4150-8c6e-80b7dc00ed26.jpeg" class="side-img">

</div>

</body>
</html>
