# viperSwift

![Swift](https://img.shields.io/badge/Swift-3.0-green.svg)

Generamba template with use DI Swinject and LightRoute:

* [LightRoute](https://github.com/SpectralDragon/LightRoute) (Helpers for creation proper module connections and routing)
* [Swinject](https://github.com/Swinject/Swinject) (Dependency injection framework for Swift)
* [SwinjectStoryboard](https://github.com/Swinject/SwinjectStoryboard) (Swinject extension for automatic dependency injection via Storyboard)

It's a shared template for [Generamba](https://github.com/rambler-digital-solutions/Generamba) code generator.


## Configure

add template to Rambafile:
```
...
- {name: viperSwift, git: 'https://github.com/petroladkin/viperSwift'}
...
```

run in root project folder:
```
> generamba template install
```


## Usage

Run command to create a new module
```
> generamba gen <module_name> viperSwift
```

by default, generamba will generate view class with a parent of UIViewController, but to customize you can add a view_type parameter.
```
> generamba gen <module_name> viperSwift [--custom_parameters view_type:<view_type>]
```

view_type:
- [x] 'view' - UIViewController has parrent for View class
- [ ] 'table' - UITableViewController has parrent for View class
- [ ] 'tabbar' - UITabBarController has parrent for View class
- [ ] 'nav' - UINavigationController has parrent for View class


The detailed information about a template structure is available in [Generamba Wiki](https://github.com/rambler-digital-solutions/Generamba/wiki/Template-Structure).
