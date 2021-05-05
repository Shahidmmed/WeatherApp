<script>
    import {onMount} from 'svelte';

    var dt = new Date();
    export var description;
    export var windSpeed;
    export var humidity;
    export var temperature;
   
</script>

<div class="uk-card-header uk-padding-top uk-margin-remove">
    <p class="uk-text-meta uk-margin-remove-top"><span id='date-time'>{dt}</span></p>
</div>
<div class="uk-card-body uk-padding-small">
  <div class="uk-flex uk-margin">
    <div class="uk-width-1-2@m uk-flex-first">
      <img class="uk-margin-remove" width="100" height="100" alt="weather icon" id="icon" >
    </div>
    <div class="uk-width-1-2@m">
      <h1 class="uk-margin-remove">{temperature} °C</h1>
    </div>
  </div>
  <h3 class="uk-margin-remove">{description}</h3>
</div>
<div class="uk-card-footer">
  <div class="uk-flex">
    <div class="uk-width-1-2@m uk-flex-first">
      Wind Speed
      <p>{windSpeed} km/h</p>
    </div>
    <div class="uk-width-1-2@m">
      Humidity
    <p>{humidity} %</p>
    </div>
  </div>
</div>