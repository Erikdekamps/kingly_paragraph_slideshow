# Kingly Paragraph Slideshow

Installs the necessary configuration for a responsive and accessible slideshow
paragraph.

## Overview

This recipe creates two new paragraph types:

1. **Kingly Slideshow:** The main container for the slideshow. It includes a
   title field and responsive settings to control the number of columns
   displayed on mobile, tablet, and desktop viewports.
2. **Kingly Slideshow Slide:** A paragraph type for an individual slide. It
   reuses the fields from the "Kingly Card" paragraph (`field_card_*`) to ensure
   consistency and data structure reuse.

The frontend rendering is powered by the `kingly_minimal:slideshow` Single
Directory Component, which uses the Splide.js library for robust accessibility,
keyboard navigation, and touch support. The individual slides are rendered using
the `kingly_minimal:card` SDC.

## Dependencies

This recipe requires the following:

- `kingly_page` recipe (for content placement)
- `kingly_paragraph_card` recipe (for field storage definitions)
- `kingly_minimal` theme (for the required SDCs)
