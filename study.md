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
    <div id="spanish">
        <h2>Do you speak Spanish?</h2>
        <div class="radio-row">
          <div class="radio">
            <input type="radio" id="spanishYes" name="spanish" value="YES" onChange="yesAnswer('smartphone')">
            <label for="yes">Yes</label><br>
          </div>
          <div class="radio">
            <input type="radio" id="spanishNo" name="spanish" value="NO" onChange="noAnswer()">
            <label for="no">No</label><br>
          </div>
        </div>
      </div>
    <div id="smartphone" style="display:none;">
        <h2>Do you have a smartphone?</h2>
        <div class="radio-row">
          <div class="radio">
            <input type="radio" id="smartphoneYes" name="smartphone" value="YES" onChange="yesAnswer('recovery')">
            <label for="yes">Yes</label><br>
          </div>
          <div class="radio">
            <input type="radio" id="smartphoneNo" name="smartphone" value="NO" onChange="noAnswer()">
            <label for="no">No</label><br>
          </div>
        </div>
      </div>
    <div id="recovery" style="display:none;">
        <h2>Are you or a loved one in recovery for substance use or mental health?</h2>
        <div class="radio-row">
          <div class="radio">
            <input type="radio" id="recoveryYes" name="recovery" value="YES" onChange="yesAnswer('help')">
            <label for="yes">Yes</label><br>
          </div>
          <div class="radio">
            <input type="radio" id="recoveryNo" name="recovery" value="NO" onChange="noAnswer()">
            <label for="no">No</label><br>
          </div>
        </div>
      </div>
    <div id="help" style="display:none;">
        <h2>Interested in helping us improve access to behavioral health services?</h2>
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
        <label for="first">First Name*</label>
        <input type="text" name="name" id="first" placeholder="First name" required>
      </div>
      <div id="phone">
        <label for="telephone">Phone Number*</label>
        <input type="telephone" name="telephone" id="telephone" placeholder="(555) 555-5555" required>
      </div>
      <div id="availability">
        <h2>When are you available to participate?</h2>
        <div style="display:flex;">
          <input type="checkbox" name="availabilityTime" value="Weekends" id="weekends" onChange="yesAnswer('submit-form-button')" required>
          <label for="weekends">Weekends</label>
        </div>
        <div style="display:flex;">
          <input type="checkbox" name="availabilityTime" value="Weekday evenings" id="evenings" onChange="yesAnswer('submit-form-button')" required>
          <label for="evenings">Weekday evenings</label>
        </div>
      </div>
      </div>
      <input type="hidden" name="_subject" id="email-subject" value="Rumbo Recruitment Form Submission">
    </fieldset>
    <input id="submit-form-button" type="submit" value="Submit" style="display:none; margin-top: 1rem;">
  </form>
  <div id="no-thanks" style="display:none;">
    <h2>Thank you for your time!</h2>
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

</script>