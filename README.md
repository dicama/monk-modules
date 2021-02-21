# monk-modules

Create your own modules for the MONK App with the MONK script:

Here is a simple example:

```
ModuleId[Module3]
ModuleName[Darmkrebs Info]
ModuleIcon[informationOutline]

Page[base=column]
WebView[https://www.krebshilfe.de/informieren/ueber-krebs/haeufige-krebsarten/darmkrebs/]
```

The syntax is pretty simple. Each line is evaluated on its own. Options/Parameters are provided in the squared bracket. Let's go through this example step by step.

Every module need an id, a name and an icon.

```
ModuleId[Module3]
```
Make sure, that your module id is unique. "Module3" as choosen in this example is not the best choice.

```
ModuleName[Darmkrebs Info]
```
The name is rather a title and can be choosen freely.

```
ModuleIcon[informationOutline]
```
The icon name can be chosen from https://materialdesignicons.com/. Please use the exact spelling from https://pub.dev/documentation/material_design_icons_flutter/latest/icon_map/iconMap.html without the quotes.

After these basic properties of the module have been defined. We can create the UI elements. In this case a simple web-site is shown. Since we are using no tabs, but rather a single page view, we are using
```
Page
```

On this page we want to show the website. So we use:

```
WebView[https://www.krebshilfe.de/informieren/ueber-krebs/haeufige-krebsarten/darmkrebs/]
```

Done. Building a simple module for MONK is super easy!

