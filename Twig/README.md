
### Implementation on the Locations Page

#### HTML Structure
The HTML structure for the Locations page (https://library.austintexas.gov/locations) includes a container for each location, displaying essential information such as the main image, name, address, and open hours.

```html
<div class="apl_location_teaser grid-col-10 grid-offset-1">
  <div class="img_container">{{ field_location_main_image }}</div>
  <div class="copy_container">
    <h2 class="field-title">{{ name_1 }}</h2>
    <div class="phone-address">{{ field_phone_num }}<br>{{ field_street_address }}</div>
    {{ drupal_view('open_hours_en', 'block_7', tid__value) }}
  </div>
</div>
```

#### Embedding Open Hours
The key function here is `{{ drupal_view('open_hours_en', 'block_7', tid__value) }}`, which calls the 'open_hours_en' Drupal View and displays it as 'block_7', passing the term ID (`tid__value`) as a parameter. This dynamically fetches and displays the relevant 'Hours' for each location.

### Open Hours View with Twig

#### Twig Template for Open Hours
The Open Hours view (`open_hours_en`) contains Twig code to format the display of hours and additional information.

```html
<div class="apl_hours">
  {{ field_hours_more_info }}
  {{ field_open_hours__ }}
</div>
```

Here, `{{ field_hours_more_info }}` and `{{ field_open_hours__ }}` are Twig variables that render the respective fields from the 'Hours' content type. This template ensures that the hours, along with any 'More Info' details, are presented in a consistent and styled manner across the site.
