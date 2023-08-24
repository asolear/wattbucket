---
hide:
  - footer
  - navigation
  - toc
---


#
</br>
</br>
</br>
<p style="font-size: 33px; color: white;font-family: 'Roboto Condensed', sans-serif;font-weight: bold;">Hacia la transición energética</p>
<p style="font-size: 22px; color: white;font-family: Roboto Condensed;">
Hola, soy Quico Roman, ingeniero (N. de colegiado 26975)  especializado en control, energías renovables, eficiencia energética y movilidad sostenible.
</p>
<p style="font-size: 22px; color: white;font-family: Roboto Condensed;">

En este blog incluyo  casos prácticos de estudios y proyectos  para el diseño de instalaciones de energía solar fotovoltaica y diseño de la infraestructura de recarga del Vehículo Eléctrico.
<p style="font-size: 22px; color: white;font-family: Roboto Condensed;">
Actualmente estoy trabajando en la reforma y conversión de motorización térmica a eléctrica de vehículos y su proceso de homologación y legalización, que pronto incluire
 </p>

</br>
</br>
</br>
</br>
</br>
</br>
<div class="collage">
    <img src="figs/asolear.png" alt="Imagen 1">
    <img src="figs/distanciaentrefilas_30.png" alt="Imagen 1">
    <img src="figs/generacioxincliancion.png" alt="Imagen 2">
    <img src="figs/generacioxincliancion.png" alt="Imagen 2">
</div>


<style> 
body { 
  background-image: url('https://github.com/asolear/assets/blob/master/imgs/fondo3.jpg?raw=true'); 
  background-repeat: no-repeat; 
  background-attachment: fixed; /* background-size: cover; */ 
  background-size: 100% 100%;
   } 

.collage {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-gap: 10px;
}
.collage img {
    max-width: 100%;
    height: auto;
    transform: rotate(0deg);
    /* Rotar la imagen 15 grados */
    transition: transform 0.3s ease;
    /* Agregar una transición suave */
}
.collage img:hover {
    transform: scale(1.1) rotate(10deg);
    /* Escalar la imagen al 110% y volver a la rotación original en el hover */
}

</style> 

<script>
    const images = document.querySelectorAll('.collage img');
    images.forEach(img => {
        img.style.transform = `rotate(${getRandomRotation()}deg) scale(${getRandomScale()})`;
    });
    function getRandomRotation() {
        return Math.floor(Math.random() * 31) - 15; // Valores de rotación aleatorios entre -15 y 15 grados
    }
    function getRandomScale() {
       return 0.8 + Math.random() * 0.4; // Valores de escala aleatorios entre 0.8 y 1.2
    }
</script>