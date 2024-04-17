# KushkiTestJERC

<!-- Tab links -->
<div class="tab">
  <button class="tablinks" onclick="openTab(event, 'Tab1')">Tab 1</button>
  <button class="tablinks" onclick="openTab(event, 'Tab2')">Tab 2</button>
  <button class="tablinks" onclick="openTab(event, 'Tab3')">Tab 3</button>
</div>

<!-- Tab content -->
<div id="Tab1" class="tabcontent">
  <h3>Contenido de la pestaña 1</h3>
  <p>Este es el contenido de la primera pestaña.</p>
</div>

<div id="Tab2" class="tabcontent">
  <h3>Contenido de la pestaña 2</h3>
  <p>Este es el contenido de la segunda pestaña.</p>
</div>

<div id="Tab3" class="tabcontent">
  <h3>Contenido de la pestaña 3</h3>
  <p>Este es el contenido de la tercera pestaña.</p>
</div>

<!-- Script para cambiar entre pestañas -->
<script>
function openTab(evt, tabName) {
  // Ocultar todos los elementos con la clase "tabcontent"
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  // Eliminar la clase "active" de todos los botones de pestaña
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  // Mostrar el contenido de la pestaña seleccionada y agregar la clase "active" al botón de la pestaña seleccionada
  document.getElementById(tabName).style.display = "block";
  evt.currentTarget.className += " active";
}
</script>
