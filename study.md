---
title: Study Recruitment
layout: page
description: Go here to sign up for one of our clinical trials
intro_image: "images/illustrations/reading.svg"
intro_image_absolute: true
intro_image_hide_on_mobile: true
sitemap: false
---

<form id="fs-frm" name="complaint-form" accept-charset="utf-8" action="https://formspree.io/f/mrgwkbjp" method="post">
  <fieldset id="fs-frm-inputs">
    <div id="recovery">
      <h2>Are you or a loved one in recovery for substance use or mental health? ¿Usted o alguien querido está en recuperación por el uso de sustancias o la salud mental?</h2>
      <div class="radio-row">
        <div class="radio">
          <input type="radio" id="recoveryYes" name="recovery" value="YES" onChange="yesAnswer('spanish')">
          <label for="yes">Yes</label><br>
        </div>
        <div class="radio">
          <input type="radio" id="recoveryNo" name="recovery" value="NO" onChange="noAnswer()">
          <label for="no">No</label><br>
        </div>
      </div>
    </div>
    <div id="spanish" style="display:none;">
      <h2 id="spanish-label">Does that person speak Spanish? ¿Esa persona habla español?</h2>
      <div class="radio-row">
        <div class="radio">
          <input type="radio" id="spanishYes" name="spanish" value="YES" onChange="yesAnswer('spanishPrimary')">
          <label for="yes">Yes / Sí</label><br>
        </div>
        <div class="radio">
          <input type="radio" id="spanishNo" name="spanish" value="NO" onChange="noAnswer()">
          <label for="no">No</label><br>
        </div>
      </div>
    </div>
    <div id="spanishPrimary" style="display:none;">
      <h2>Do you read better in Spanish? ¿Lees mejor en español?</h2>
      <div class="radio-row">
        <div class="radio">
          <input type="radio" id="spanishPrimaryYes" name="spanishPrimary" value="YES" onChange="spanishLabels()">
          <label for="yes">Yes / Sí</label><br>
        </div>
        <div class="radio">
          <input type="radio" id="spanishPrimaryNo" name="spanishPrimary" value="NO" onChange="yesAnswer('adult')">
          <label for="no">No</label><br>
        </div>
      </div>
    </div>
    <div id="adult" style="display:none;">
      <h2 id="adult-label">Are you an adult over the age of 18?</h2>
      <div class="radio-row">
        <div class="radio">
          <input type="radio" id="adultYes" name="adult" value="YES" onChange="yesAnswer('smartphone')">
          <label for="yes">Yes / Sí</label><br>
        </div>
        <div class="radio">
          <input type="radio" id="adultNo" name="adult" value="NO" onChange="noAnswer()">
          <label for="no">No</label><br>
        </div>
      </div>
    </div>
    <div id="smartphone" style="display:none;">
      <h2 id="smartphone-label">Do you have a smartphone?</h2>
      <div class="radio-row">
        <div class="radio">
          <input type="radio" id="smartphoneYes" name="smartphone" value="YES" onChange="yesAnswer('help')">
          <label for="yes">Yes</label><br>
        </div>
        <div class="radio">
          <input type="radio" id="smartphoneNo" name="smartphone" value="NO" onChange="noAnswer()">
          <label for="no">No</label><br>
        </div>
      </div>
    </div>
    <div id="help" style="display:none;">
      <h2 id="help-label">Interested in helping us improve access to behavioral health services?</h2>
      <div class="radio-row">
        <div class="radio">
          <input type="radio" id="helpYes" name="help" value="YES" onChange="yesAnswer('full_form')">
          <label for="yes">Yes</label><br>
        </div>
        <div class="radio">
          <input type="radio" id="helpNo" name="help" value="NO" onChange="noAnswer()">
          <label for="no">No</label><br>
        </div>
      </div>
    </div>
    <div id="full_form" style="display:none;">
      <div id="name">
        <label for="first" id="name-label">First Name*</label>
        <input type="text" name="name" id="first" placeholder="First name / Primer nombre" required>
      </div>
      <div id="phone">
        <label for="telephone" id="phone-label">Phone Number*</label>
        <input type="telephone" name="telephone" id="telephone" placeholder="(555) 555-5555" required>
      </div>
      <div id="availability">
        <label for="contact" id="availability-label">When is a good time to contact you?*</label>
        <input type="text" name="contact" id="contact" placeholder="Monday evenings, for example / Los lunes por la tarde, por ejemplo." required>
      </div>
    </div>
    <input type="hidden" name="_subject" id="email-subject" value="Rumbo Recruitment Form Submission">
  </fieldset>
  <input id="submit-form-button" type="submit" value="Submit / Enviar" style="display:none; margin-top: 1rem;">
</form>
<div id="no-thanks" style="display:none;">
  <h2 id="nothanks-label">Thank you for your time -- unfortunately, we're looking for somebody else!</h2>
</div>

  <style>/* reset */
  #fs-frm input,
  #fs-frm select,
  #fs-frm textarea,
  #fs-frm fieldset,
  #fs-frm optgroup,
  #fs-frm label,
  #fs-frm #card-element:disabled {
    font-family: inherit;
    font-size: 100%;
    color: inherit;
    border: none;
    border-radius: 0;
    display: block;
    width: 100%;
    padding: 0;
    margin: 0;
    -webkit-appearance: none;
    -moz-appearance: none;
  }
  #fs-frm label,
  #fs-frm legend,
  #fs-frm ::placeholder {
    font-size: .825rem;
    padding-top: .2rem;
    display: flex;
    align-items: baseline;
  }
  
  /* border, padding, margin, width */

  #fs-frm input,
  #fs-frm select,
  #fs-frm textarea,
  #fs-frm #card-element {
    border: 1px solid rgba(0,0,0,0.2);
    background-color: rgba(255,255,255,0.9);
    padding: .75em 1rem;
    margin-bottom: 1.5rem;
  }
  #fs-frm input:focus,
  #fs-frm select:focus,
  #fs-frm textarea:focus {
    background-color: white;
    outline-style: solid;
    outline-width: thin;
    outline-color: gray;
    outline-offset: -1px;
  }
  #fs-frm [type="text"],
  #fs-frm [type="email"] {
    width: 100%;
  }
  #fs-frm [type="button"],
  #fs-frm [type="submit"],
  #fs-frm [type="reset"] {
    width: auto;
    cursor: pointer;
    -webkit-appearance: button;
    -moz-appearance: button;
    appearance: button;
  }
  #fs-frm [type="button"]:focus,
  #fs-frm [type="submit"]:focus,
  #fs-frm [type="reset"]:focus {
    outline: none;
  }
  #fs-frm [type="submit"],
  #fs-frm [type="reset"] {
    margin-bottom: 0;
  }
  #fs-frm select {
    text-transform: none;
  }
  
  #fs-frm [type="checkbox"] {
    -webkit-appearance: checkbox;
    -moz-appearance: checkbox;
    appearance: checkbox;
    display: inline-block;
    width: auto;
    margin: 0 .5em 0 0 !important;
  }
  
  #fs-frm [type="radio"] {
    -webkit-appearance: radio;
    -moz-appearance: radio;
    appearance: radio;
    margin-bottom: 0 !important;
    margin-right: 3em;
    width: unset;
  }
  
  /* address, locale */
  #fs-frm fieldset.locale input[name="city"],
  #fs-frm fieldset.locale select[name="state"],
  #fs-frm fieldset.locale input[name="postal-code"] {
    display: inline;
  }
  #fs-frm fieldset.locale input[name="city"] {
    width: 52%;
  }
  #fs-frm fieldset.locale select[name="state"],
  #fs-frm fieldset.locale input[name="postal-code"] {
    width: 20%;
  }
  #fs-frm fieldset.locale input[name="city"],
  #fs-frm fieldset.locale select[name="state"] {
    margin-right: 3%;
  }
  </style>

<script>

var labelStrings = {
  smartphone: {
    english: 'Do you have a smartphone?',
    spanish: '¿Tiene un smartphone?'
  },
  adult: {
    english: 'Are you an adult over the age of 18?',
    spanish: '¿Eres adulto mayor de 18 años?'
  },
  help: {
    english: 'Interested in helping us improve access to behavioral health services?',
    spanish: '¿Está interesado en ayudarnos a mejorar el acceso a los servicios de salud mental y tratamiento de adicciones?'
  },
  name: {
    english: 'First Name*',
    spanish: 'Primer nombre*'
  },
  phone: {
    english: 'Phone Number*',
    spanish: 'Número de teléfono*'
  },
  availability: {
    english: 'When is a good time to contact you?*',
    spanish: '¿Cuándo es un buen momento para contactarlo?*'
  },
  nothanks: {
    english: 'Thank you for your time -- unfortunately, we\'re looking for somebody else!',
    spanish: '¡Gracias por su tiempo, pero estamos buscando a otra persona!'
  }
}

var speaksSpanish = false;

function yesAnswer(selector) {
  var element = document.getElementById(selector);
  element.style.display = 'block';
}

function noAnswer() {
  var formElement = document.getElementById('fs-frm');
  formElement.style.display = 'none';

  var noThanksElement = document.getElementById('no-thanks');
  noThanksElement.style.display = 'block';
}

function spanishLabels() {
  // handle translations
  for (var label in labelStrings) {
    document.getElementById(label + '-label').innerHTML = labelStrings[label]['spanish'];
  }
  
  // show element
  var element = document.getElementById('adult');
  element.style.display = 'block';
}

var contactElement = document.getElementById('contact');
contactElement. addEventListener("input", (event) => {
  var submit = document.getElementById('submit-form-button');
  submit.style.display = 'block';
});

</script>