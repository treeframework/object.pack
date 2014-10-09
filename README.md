# Pack

The Pack object simply causes any number of elements pack up horizontally
to automatically fill an equal, fluid width of their parent.

## Dependencies

The Pack object depends on two other module:

[settings.defaults](https://github.com/treeframework/settings.defaults)
[tools.functions](https://github.com/treeframework/tools.functions)

If you install the Pack object using Bower, you will get these dependencies at
the same time. If not using Bower, please be sure to install and `@import` these
dependencies in the relevant way.

## Installation

The recommended way to install is Bower, but you can install Pack module via a
Git Submodule, or copy and paste.

### Install using Bower:

    $ bower install --save tree-pack

Once installed, `@import` into your project in its Object layer:

    @import "bower_components/tree-pack/object.pack";

### Install as a Git Submodule:

    $ git submodule add git@github.com:treeframework/object.pack.git

### Install via file download

The least recommended option dor installation is to simply download
`_object.pack.scss` into your project and `@import` it into your project in its
Objects layer.

## Usage

Basic usage of the Pack object uses the required classes:

    <div class="pack">
        <div class="pack__item">
            Foo
        </div>
        <div class="pack__item">
            Bar
        </div>
        <div class="pack__item>
            Baz
        </div>
    </div>

The only valid children of the `.pack` node are `.pack__item`s.

## Options

Other, optional classes can supplement the required base classes:

* `.pack--auto`: cause packed items to have an automatically determined,
  non-equal width.
* `.pack--[tiny|small|large|huge]`: alter the gutter between pack items.
* `.pack--rev`: reverse the rendered horizontal order of packed items.
* `.pack--[middle|bottom]`: align packed items to the middles or bottoms of each
  other.

For example:

    <div class="pack  pack--small  pack-rev">
        <div class="pack__item>
            Foo
        </div>
        <div class="pack__item>
            Bar
        </div>
        <div class="pack__item>
            Baz
        </div>
    </div>

## Credits

* **[inuitcss](https://github.com/inuitcss)** Powerful, Sass-based, OOCSS
framework designed with scalability and performance in mind.
