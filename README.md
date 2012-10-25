INSTALLATION

- Install libraries module (dependency).
- Download jQuery-Placeholder library from https://github.com/danielstocks/jQuery-Placeholder
- Place this library in sites/[all/sitename/default]/libraries/placeholder
  so the jquery.placeholder.js is located at sites/[all/sitename/default]/libraries/placeholder/jquery.placeholder.js

USAGE

- Add a '#placeholder' key or a 'placeholder' element to the '#attributes'
  array to textfield or textareas.

E.g.

function placeholder_form_search_block_form_alter(&$form, &$form_state) {
  $form['search_block_form']['#placeholder'] = t('Search here');
  // or ....
  $form['search_block_form']['#attributes']['placeholder'] = t('Search here');
}
