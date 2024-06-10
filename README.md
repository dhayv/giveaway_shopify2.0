# Shopify Giveaway Landing Page

## Table of Contents

- [Project Overview](#project-overview)
- [Why No Stylesheet?](#why-no-stylesheet)
- [Importance of No Header and Footer](#importance-of-no-header-and-footer)
- [Implementation Steps](#implementation-steps)
  - [Create a New Template File](#create-a-new-template-file)
  - [Edit the Template File](#edit-the-template-file)

## Project Overview

This project focuses on creating a streamlined Shopify landing page specifically designed for giveaways. The goal is to maximize user engagement and conversion by eliminating distractions such as headers and footers. The landing page leverages Shopify's native drag-and-drop feature for content placement and styling, simplifying the design process and making additional stylesheets unnecessary.

## Why No Stylesheet?

By utilizing Shopify's built-in drag-and-drop editor, we can easily manage the page's layout and design directly within the Shopify admin interface. This approach has several benefits:

- **Ease of Use**: Non-developers can easily update and manage the content without needing to write or modify CSS.
- **Consistency**: Ensures the design remains consistent with other parts of the Shopify store that also use the drag-and-drop editor.
- **Performance**: Reduces the need for additional HTTP requests, as no external stylesheet needs to be loaded.

## Importance of No Header and Footer

For a giveaway landing page, the primary goal is to focus the user's attention on the giveaway itself. Headers and footers can distract from this objective by:

- **Reducing Distractions**: Without a header and footer, there are fewer elements to divert the user's attention away from the main content.
- **Streamlined Experience**: Creates a more immersive and focused user experience, increasing the likelihood of participation in the giveaway.
- **Enhanced Conversion Rates**: By minimizing navigation options, users are more likely to complete the desired action (e.g., entering the giveaway) rather than browsing away.

## Implementation Steps

### Create a New Template File

1. Navigate to `Online Store > Themes > Actions > Edit code` in your Shopify Admin.
2. In the `Templates` directory, create a new file named `page.giveaway.liquid`.

### Edit the Template File

Add the following code to the `page.giveaway.liquid` file to remove the header and footer:

```liquid
{% comment %}
This template is used for the giveaway landing page.
{% endcomment %}

{% layout none %}

<!-- Your giveaway content goes here -->

<!-- End of giveaway content -->
