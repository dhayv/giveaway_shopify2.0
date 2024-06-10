# Shopify Giveaway Landing Page

## Table of Contents
- [Project Overview](#project-overview)
- [Why No Stylesheet?](#why-no-stylesheet)
- [Importance of No Header and Footer](#importance-of-no-header-and-footer)
- [Implementation Steps](#implementation-steps)
  - [Create a Default Page and Edit in Shopify](#create-a-default-page-and-edit-in-shopify)
  - [Remove Header and Footer](#remove-header-and-footer)
  - [Add Client's Logo](#add-clients-logo)

## Project Overview
This project focuses on creating a Shopify landing page specifically for a giveaway, with the intent to maximize user engagement by eliminating distractions such as headers and footers. The page is designed using unique HTML code to create a Shopify Liquid theme page, leveraging Shopify's native drag-and-drop feature for content placement and styling, which makes additional stylesheets unnecessary.

## Why No Stylesheet?
By using Shopify's built-in drag-and-drop editor, we can efficiently manage the page's layout and design directly within the Shopify admin interface. This approach offers several advantages:

- **Ease of Use**: Non-developers can update and manage the content effortlessly without needing to write or modify CSS.
- **Consistency**: Ensures the design remains consistent with other parts of the Shopify store that also utilize the drag-and-drop editor.
- **Performance**: Reduces the need for additional HTTP requests, as no external stylesheet needs to be loaded, enhancing page load times.

## Importance of No Header and Footer
For a giveaway landing page, the primary goal is to capture the user's attention and direct it towards the giveaway itself. Removing headers and footers helps achieve this by:

- **Reducing Distractions**: Without a header and footer, there are fewer elements to divert the user's attention away from the main content.
- **Streamlined Experience**: Creates a more immersive and focused user experience, increasing the likelihood of participation in the giveaway.
- **Enhanced Conversion Rates**: By minimizing navigation options, users are more likely to complete the desired action (e.g., entering the giveaway) rather than navigating away.

## Implementation Steps

### Create a Default Page and Edit in Shopify

1. Start by creating a default page in Shopify and then navigate to the Shopify theme editor.
2. Select the newly created page and add a custom Liquid section.

### Remove Header and Footer

In the custom Liquid section, paste the following code to hide the header and footer elements:

```html
<style>
#shopify-section-header, .shopify-section-header, shopify-section-header {display:none !important;}
#announcement-bar, .announcement-bar, announcement-bar {display:none !important;}
#header, .header, header {display:none !important;}
#footer, .footer, footer {display:none !important;}
</style>

This code removes all the specified elements, providing a blank canvas to focus on the giveaway content.

## Add Client's Logo
