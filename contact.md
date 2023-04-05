---
title: Contact
subtitle: Please follow the instructions. I will try to read you as soon as posible
layout: page
---

<div class="container">
  <h1>Contact Form</h1>
  <form target="_blank" action="https://formsubmit.co/29a3b05b7bde654a6e5d5100857cf797" method="POST" id="mi-formulario">
    <div class="form-group">
      <div class="form-row">
        <div class="col">
          <input type="text" name="name" class="form-control" placeholder="Full Name" required>
        </div>
        <div class="col">
          <input type="email" name="email" class="form-control" placeholder="Email Address" required>
        </div>
      </div>
    </div>
    <div class="form-group">
      <textarea placeholder="Your Message" class="form-control" name="message" rows="10" required></textarea>
    </div>
    <button type="submit" class="btn btn-lg btn-dark btn-block">Submit Form</button>
    
  </form>
</div>
<script>
  document.getElementById("mi-formulario").addEventListener("submit", function() {
    // Obtén todos los elementos del formulario
    var elementosForm = this.elements;
    
    // Recorre todos los elementos del formulario
    for (var i = 0; i < elementosForm.length; i++) {
      // Si el elemento es un campo de texto o correo electrónico
      if (elementosForm[i].type === "text" || elementosForm[i].type === "email" || elementosForm[i].name === "message") {
        // Borra el valor del campo
        elementosForm[i].value = "";
      }
    }
  });
</script>

