## 
![](https://github.com/asolear/assets/blob/master/imgs/cabecerag.png?raw=true)


<center><h1 style="color:orange;  
  font-size: large">Oficina Técnica de Autoconsumo</h1></center>
<center><p style="color:red;  
  font-size: xx-small"> :fontawesome-solid-file-pen:.-Su documentacion (.pdf/xls/dxf) a medida en  minutos !</p></center>

<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"
    integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin="" />
<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"
    integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>




<style>
body {
    /* background-image: url('Wavy_REst-03_Single-07.jpg');  */
    /* background-image: url('assets/images/logo.svg');  */
    /* background-image: url('https://github.com/asolear/assets/blob/master/imgs/cabecerag.png?raw=true');  */
    background-repeat: no-repeat; 
    background-attachment: fixed; 
    background-size: 100% 100%; 
    } 
select {
    width: 100%;
    padding: 12px 20px;
    margin: 8px 0;
    color: black;
    display: inline-block;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;
    font-size: 24px;
    }
</style>

<div id="map" style="width: 100%; height: 300px;"></div>
<label>Ubicación *</label>



<form action="mailto:info@wattbucket.com?subject=QR " method="post"enctype="text/plain">
    <input type="hidden" name="correo_Documento" id="correo_Documento"  value=""><br>
    <input type="hidden" name='Ubicacion_latitud' class="form-control" id="lat" value="40.41630407781033">
    <input type="hidden" name='Ubicacion_longitud' class="form-control" id="lng" value="-3.703777670925774">

                    
         <label>Consumo Anual (kWh)</label><br><select name="Electrico_Consumo Anual (kWh)" class="form-control" id="Electrico_Consumo Anual (kWh)" required>  <option value="     0 -  5.000">     0 -  5.000</option>  <option value=" 5.000 -  8.000"> 5.000 -  8.000</option>  <option value=" 8.000 - 10.000"> 8.000 - 10.000</option>  <option value="10.000 - 15.000">10.000 - 15.000</option>  <option value="15.000 - 30.000">15.000 - 30.000</option>  <option value="30.000 - 80.000">30.000 - 80.000</option>  <option value="80.000 - 50.000">80.000 - 50.000</option> </select> <br> <label>Nombre</label><br> <input type="text" id="Tecnico_Nombre" name="Tecnico_Nombre" > <br> <label>Titulación</label><br> <input type="text" id="Tecnico_Titulación" name="Tecnico_Titulación" > <br> <label>representante</label><br><select name="Incentivo_representante" class="form-control" id="Incentivo_representante" required>  <option value="representante legal de la instalador instaladora">representante legal de la instalador instaladora</option>  <option value="beneficiario">beneficiario</option>  <option value="entidad adherida">entidad adherida</option> </select> <br> 

<input type="file" name="archivo">
<br><br><label><input type="checkbox" class="agree" required> Acepto la Política de
    Privacidad</label><br><input type="submit" style="width:100%;height: 60px;background-color: #4CAF50"
    value="✉️ eMAIL"><br>
</form>




<script>

    var map = L.map('map').setView([40.41630407781033, -3.703777670925774], 13);

    var tiles = L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
        attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
    }).addTo(map);
    var marker = L.marker([40.41630407781033, -3.703777670925774]).addTo(map).openPopup();
    map.on('click', function (e) {
        if (marker) {
            map.removeLayer(marker);
        }
        marker = new L.Marker(e.latlng).addTo(map).openPopup();
        document.getElementById('lat').value = e.latlng.lat;
        document.getElementById('lng').value = e.latlng.lng;
    });
</script>


        