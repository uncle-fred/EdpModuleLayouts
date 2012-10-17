EdpModuleLayouts
================
Version 1.0 Created by Evan Coury

Introduction
------------

EdpModuleLayouts is a very simple ZF2 module (less than 20 lines) that simply
allows you to specify alternative layouts to use for each module.

Usage
-----

Using EdpModuleLayouts is very, very simple. In any module config or autoloaded
config file simply specify the following:

```php
array(
    'module_layouts' => array(
        'ModuleName' => 'layout/some-layout',
    ),
);
```

Make sure you name each module layout file differently. As an example:
Module called "Dialogue" would have its layout file "ApplicationName/module/Dialogue/view/layout/dialogue.phtml" and configuration set to
```php
    'module_layouts' => array(
        'Dialogue' => 'layout/dialogue.phtml',
    ),
```
And module called "Moderation" would have its layout file "ApplicationName/module/Moderation/view/layout/moderation.phtml" and configuration set to
```php
    'module_layouts' => array(
        'Moderation' => 'layout/moderation.phtml',
    ),
```
That's it!