# Responsive File Manager for TinyMCE 6.x

This repository provides a fully fixed version of Responsive File Manager that can be used in TinyMCE 6. If you’re looking to manage files and images within your TinyMCE editor, this solution will help you achieve that seamlessly.

## Installation

*Note: MAKE SURE `gd` extension is enabled on your server.*

1. **Folder Placement:** Start by dropping the  `filemanager` folder into your root directory, so it should be along side `tinymce` folder, not inside it.
2. **Add Plugins:** Add the `responsivefilemanager` plugin to your TinyMCE plugins folder and it's configuration. Make sure it’s included in the list of plugins.
3. **Specify External File Manager Path:** Inside your TinyMCE initialization, add the parameter `external_filemanager_path` and specify the path to the `filemanager` folder. For example:

    ```javascript
    tinymce.init({
        // Other configurations...
        plugins: 'responsivefilemanager',
        external_filemanager_path: '/path/to/filemanager/',
        // Other settings...
    });
    ```

    Replace `/path/to/filemanager/` with the actual path to `filemanager` from root directory.

## Usage

Once you’ve completed the installation steps, you’ll be able to use the Responsive File Manager seamlessly within your TinyMCE editor. It allows you to upload, manage and insert files, links and images directly from the editor interface. It can also be used to enter multiple pictures at a time into the editor. To Use **multi-image** feature, click on upload icon from editor and choose multiple pictures, then press Select.

You can set access keys via `config.php` inside the filemanager folder. enable the keys, add keys to the `array()`, and put the same key inside `plugin.min.js` of responsivefilemanager.

*Note: This README assumes that you have already set up TinyMCE 6.x and have the latest PHP version installed on your server.*

As of time of testing, PHP 8.2.15 and TinyMCE 6.8.3 were used

Link to Original Creator's outdated version: [https://github.com/trippo/ResponsiveFilemanager].

