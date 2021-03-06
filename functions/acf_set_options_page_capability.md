---
title: acf_set_options_page_capability()
description: Modifies the default Options Page capability setting.
category: functions
group: Deprecated
deprecated: true
---

## Description
[tip]
This function has been deprecated. Please use the [acf/options_page/settings](https://www.advancedcustomfields.com/resources/acf-options_page-settings/) filter instead.
[/tip]

Modifies the default Options Page capability setting.

The term ‘capability’ refers to the user roles and permissions that grant access to the Options Page. You can learn more about [capability settings here](http://codex.wordpress.org/Roles_and_Capabilities).

## Requirements
- [Options Page Add-on](https://www.advancedcustomfields.com/add-ons/options-page/) version 1.1.0 or later.

## Parameters
```
acf_set_options_page_capability( $capability );
```
- `$capability` *(string)* *(Required)* The capability for the default Options Page. Defaults to 'edit_posts'.

## Example
This example demonstrates how to change the default Options Page capability to 'manage_options'.

#### functions.php
```
if( function_exists('acf_set_options_page_capability') ) {
	acf_set_options_page_capability('manage_options');
}
```
