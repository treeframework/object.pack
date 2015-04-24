# Pack

The `pack` object simply causes any number of elements pack up horizontally
to automatically fill an equal, fluid width of their parent.

## Dependencies

The `pack` object depends on two other modules:

* [settings.defaults](https://github.com/treeframework/settings.defaults)
* [tools.functions](https://github.com/treeframework/tools.functions)

If you install the `pack` object using Bower or npm, you will get these 
dependencies at the same time. If not using Bower or npm, please be sure to 
install and `@import` these dependencies in the relevant way.

## Installation

You can install `pack` module via Bower, npm, or copy and paste.

### Install using Bower:

```sh
$ bower install tree-pack --save
```

Once installed, `@import` into your project in its Object layer:

```scss
@import "bower_components/tree-pack/object.pack";
```

### Install using npm:

```sh
$ npm install tree-pack --save
```

### Install via file download

The least recommended option for installation is to simply download
`_object.pack.scss` into your project and `@import` it into your project in its
Objects layer.

## Usage

Basic usage of the Pack object uses the required classes:

```html
<div class="o-pack">
    <div class="o-pack__item">
        Foo
    </div>
    <div class="o-pack__item">
        Bar
    </div>
    <div class="o-pack__item">
        Baz
    </div>
</div>
```

The only valid children of the `.o-pack` node are `.o-pack__item`s.

## Options

Other, optional classes can supplement the required base classes:

* `.o-pack--auto`: cause packed items to have an automatically determined,
  non-equal width.
* `.o-pack--[tiny|small|large|huge]`: alter the gutter between pack items.
* `.o-pack--rev`: reverse the rendered horizontal order of packed items.
* `.o-pack--[middle|bottom]`: align packed items to the middles or bottoms of each
  other.

For example:

```html
<div class="o-pack  o-pack--small  o-pack-rev">
    <div class="o-pack__item">
        Foo
    </div>
    <div class="o-pack__item">
        Bar
    </div>
    <div class="o-pack__item">
        Baz
    </div>
</div>
```

## Credits

* **[inuitcss](https://github.com/inuitcss)** Powerful, Sass-based, OOCSS
framework designed with scalability and performance in mind.
