# Bootstrap Toolbox Block to Card Module

**Module Name**: Bootstrap Toolbox Block to Card  
**Module Version**: 1.0  
**Drupal Compatibility**: 9.x, 10.x  
**Author**: [Your Name or Company]  
**License**: GPL-2.0+

## Description

The **Bootstrap Toolbox Block to Card** module provides a mechanism to theme blocks as Bootstrap cards, allowing for enhanced visual styling and customization within Drupal's Layout Builder and standard block forms. This module integrates seamlessly with the Bootstrap Toolbox, offering options to select card styles, header styles, and body styles for individual blocks.

## Features

- **Card Theming**: Enable or disable card theming for blocks.
- **Style Selection**: Choose from predefined styles for the card, header, and body.
- **Layout Builder Integration**: Supports theming of blocks directly within Layout Builder.
- **Third-Party Settings**: Uses Drupal's third-party settings API for storing and retrieving block configuration.

## Installation

1. Download and place the module in the `/modules/custom` directory of your Drupal installation.
2. Enable the module via the Drupal admin UI or using Drush:

   ```bash
   drush en bt_block_card```
3. Clear the cache
   ```drush cr```

## Usage
### Configuring a Block
1. Navigate to the block settings or Layout Builder configuration for a block.
2. Under the Bootstrap Toolbox vertical tab, you'll find the "Theme as a card" section.
3. Check the Theme as a card option to apply card styling to the block.
4. Select the desired styles for the card, header, and body from the available options.
5. Save the block configuration.
### Customization
To customize the available styles, you can modify the options provided by the Bootstrap Toolbox utility service. The module expects the styles to be defined within the Bootstrap Toolbox's configuration.

## Templates
The module includes a Twig template (bt-block-card.html.twig) for rendering blocks as cards. This template can be overridden in your theme if needed.

## Hooks

hook_block_view_alter()
Alters the block view to apply card theming if enabled in the block's configuration.

hook_preprocess_bt_block_card()
Preprocesses variables for the card-themed block template.

hook_preprocess_layout()
Preprocesses layout variables to apply card theming within Layout Builder.

## Requirements

- **Drupal 9+**: Minimum required version.
- **Bootstrap**: Must be included in your theme or site, as the carousel depends on this CSS framework.

## Contributing

Contributions, bug reports, and feature requests are welcome on the project page on
 [Drupal.org](https://www.drupal.org).

## Maintenance

The module is maintained by [Carlos Espino](https://www.drupal.org/u/carlos-espino).
You can contact me via the contact form on my Drupal.org profile page.
