
# Displaying Open Hours and More Info on library.austintexas.gov

## Overview
This document outlines the implementation and usage of the 'Hours' content type on the library.austintexas.gov website, particularly focusing on displaying operational hours and additional information for library locations.

## Content Type: Open Hours
- **Fields**: Includes fields for 'More Info', a date range for activation, applicable locations, and daily open and closing hours.
- **Dynamic Display**: The most recently applicable 'Hours' content is shown on relevant location pages.
- **Scheduling**: Allows for scheduling new hours to take effect later or for short periods, with automatic reversion to previous settings.

## Module Used
- **Office Hours**: This module (Machine name: office_hours, Version: 8.x-1.8) defines a 'weekly office hours' field type, used to specify when an Entity is open or closed.

## Embedding Open Hours
- **Drupal Views**: The 'Hours' content is typically embedded through Drupal Views, which creates a block or is sometimes added as an extra field within a Drupal View.

## 'More Info' Section
- **Usage**: This section is particularly useful for explaining temporary closures or special notices, ensuring the public is well informed about any changes in operational hours.

## Updating Open Hours
- **Adding a New Node**: Administrators can add new 'Hours' content by navigating to [Add Hours Node](https://library.austintexas.gov/node/add/open_hours).
- **Editing Existing Content**: To edit existing 'Hours', careful attention should be paid to when it's set to display and which locations it affects. 
