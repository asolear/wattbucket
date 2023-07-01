# Justificante BASES REGULADORAS  PARA INSTALACIONES FOTOVOLTAICAS <a href="../111_Incentivos_Justificante BASES REGULADORAS  PARA INSTALACIONES FOTOVOLTAICAS.pdf">   :fontawesome-solid-file-pdf:</a>,<a href="../111_Incentivos_Justificante BASES REGULADORAS  PARA INSTALACIONES FOTOVOLTAICAS">    :fontawesome-solid-file:</a>
<body>
    <div id="map" style="width: 100%; height: 300px;"></div><label>Ubicación *</label>
    <script data-require="leaflet@0.7.3" data-semver="0.7.3"
        src="https://cdnjs.cloudflare.com/ajax/libs/leaflet/0.7.3/leaflet.js"></script>
    <link data-require="leaflet@0.7.3" data-semver="0.7.3" rel="stylesheet"
        href="//cdnjs.cloudflare.com/ajax/libs/leaflet/0.7.3/leaflet.css" />
    <style>
        input[type=text],
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

        input[type=submit] {
            width: 100%;
            background-color: #4CAF50;
            color: black;
            padding: 14px 20px;
            margin: 8px 0;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 24px;
        }

        input[type=submit]:hover {
            background-color: #45a049;
        }
    </style>
    
    <form action="mailto:info@wattbucket.com?subject=QR Justificante BASES REGULADORAS  PARA INSTALACIONES FOTOVOLTAICAS" method="post" enctype="text/plain">
        <input type="hidden" name="correo_Documento" id="correo_Documento"  value="Justificante BASES REGULADORAS  PARA INSTALACIONES FOTOVOLTAICAS"><br>
        <input type="hidden" name='Ubicacion_latitud' class="form-control" id="lat" value="40.41630407781033">
        <input type="hidden" name='Ubicacion_longitud' class="form-control" id="lng" value="-3.703777670925774">

 <h3>Tecnico</h3> <label>Nombre</label><br> <input type="text" id="Tecnico_Nombre" name="Tecnico_Nombre" > <br> <label>Titulación</label><br> <input type="text" id="Tecnico_Titulación" name="Tecnico_Titulación" > <br> <label>N.I.F.</label><br> <input type="text" id="Tecnico_N.I.F." name="Tecnico_N.I.F." > <br> <label>Empresa</label><br> <input type="text" id="Tecnico_Empresa" name="Tecnico_Empresa" > <br> <label>N.I.F. Empresa</label><br> <input type="text" id="Tecnico_N.I.F. Empresa" name="Tecnico_N.I.F. Empresa" > <br> <label>Direccion</label><br> <input type="text" id="Tecnico_Direccion" name="Tecnico_Direccion" > <br> <label>Poblacion</label><br> <input type="text" id="Tecnico_Poblacion" name="Tecnico_Poblacion" > <br> <label>Provincia</label><br> <input type="text" id="Tecnico_Provincia" name="Tecnico_Provincia" > <br> <label>Correo electrónico</label><br> <input type="text" id="Tecnico_Correo electrónico" name="Tecnico_Correo electrónico" > <br> <label>Teléfono</label><br> <input type="text" id="Tecnico_Teléfono" name="Tecnico_Teléfono" > <br> 
            <input type="file" name="archivo">
        <br><br><label><input type="checkbox" class="agree" required> Acepto la Política de
            Privacidad</label><br><input type="submit" style="width:100%;height: 60px;background-color: #4CAF50"
            value="✉️ eMAIL"><br>
    </form>
        
    <script>
        var tileLayer = new L.TileLayer('http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
            'attribution': 'Map data © <a href="http://openstreetmap.org">OpenStreetMap</a> contributors'
        });
        var map = new L.Map('map', {
            'center': [40.41630407781033, -3.703777670925774],
            'zoom': 5,
            'layers': [tileLayer]
        });
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
</body>
            