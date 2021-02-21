# monk-modules
#### Create your own modules for the MONK App with the MONK script. :smiley: Its fun!

> Check our <a href="https://github.com/dicama/monk-modules/blob/main/CONTRIBUTING.MD">Contribution Guidelines</a> to get you started :rocket:
> 

Here is a simple example:

## Example: Create Your Own Module (The Webviewer)

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
Page[base=column]
```
Here we set the paramter `base=column`. This is needed if we want to embed a single WebView element. If we would like to embed multiple UI elements, we would rather use `base=list` but this is not the case here. :-)

On this page we want to show the website. So we use:

```
WebView[https://www.krebshilfe.de/informieren/ueber-krebs/haeufige-krebsarten/darmkrebs/]
```

Done. Building a simple module for MONK is super easy :star_struck:!

### Acknowledgment

We gratefully acknowledge strong support by the Open Knowledge Foundation Germany e.V., Prototype Fund, German Federal Ministry of Research and Education, Health Hackers e.V. as well as everyone who is contributing to this project by providing feedback, ideas and further visionary thoughts.

<p class="aligncenter">
       <img align="middle" src="https://github.com/dicama/dicama/blob/dicama-imgs-1/acknowledgments.svg" width="800">
 </p>
   
### License
All work provided is published under the terms of the MIT Licence Agreement.
See <a href="https://github.com/dicama/monk-modules/blob/main/LICENSE">DiCaMa Licence Agreement</a> for more information.
