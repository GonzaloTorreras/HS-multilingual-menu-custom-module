# Multilingual menu module
This module is commonly used inside the header (global module). There you can choose one menu per language. So it basically allows you to have one template/header/footer for as many languages as you need.

Did I mention it also works in the system pages? :)


You only need a repeatable group that will create the dictionary we need (in our case the group slug is: `menu_by_lang`):
The `lang_slug` will be the slug that will be compare to, while the `menu_id` will be the asociated menu to such slug/lang.
```
{
  [
    "lang_slug": "es/",
    "menu_id": "1234"
  ],
  [
    "lang_slug": "en/",
    "menu_id": "0000"
  ]
}
```

*Notice: the last element/row will be the default element to display if there is no match with the slug *
