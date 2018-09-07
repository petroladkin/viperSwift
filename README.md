# viperSwift

![Swift](https://img.shields.io/badge/Swift-4.1-brightgreen.svg)

Generamba template with use Swinject and SwinjectStoryboard for DI, LightRoute for routing, Quick and Nimble for testing:

* [Swinject](https://github.com/Swinject/Swinject) (Dependency injection framework for Swift)
* [SwinjectStoryboard](https://github.com/Swinject/SwinjectStoryboard) (Swinject extension for automatic dependency injection via Storyboard)
* [LightRoute](https://github.com/SpectralDragon/LightRoute) (Helpers for creation proper module connections and routing)
* [Quick](https://github.com/Quick/Quick) (The Swift (and Objective-C) testing framework)
* [Nimble](https://github.com/Quick/Nimble) (A Matcher Framework for Swift and Objective-C)

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
- [x] 'view' - view class has parent UIViewController class
- [ ] 'table' - view class has parent UITableViewController class
- [ ] 'tabbar' - view class has parent UITabBarController class
- [ ] 'nav' - view class has parent UINavigationController class


The detailed information about a template structure is available in [Generamba Wiki](https://github.com/rambler-digital-solutions/Generamba/wiki/Template-Structure).
