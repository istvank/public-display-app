# Public Display App

This is an HTML element plus application shell for creating simple HTML-based content for public displays.

## Usage

To change the content of the slides, edit the `src/public-display-app.html` file:
```
<public-display interval="2000">
  <div style="text-align: center;" slide><h1>Welcome to this Display!</h1></div>
  <img src="http://lorempixel.com/1920/1080/sports/2" slide/>
  <img src="http://lorempixel.com/1920/1080/sports/3" slide/>
</public-display>
```
Any HTML tag put in the `public-display` tag is rendered as its own slide, as long as it has the `slide` attribute.
The duration the slides are shown each can be set with the `interval` attribute as value in milliseconds.
It defaults to 5000 ms.
In the example above, it is set to 2 seconds.

## Running the Application

### Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.

### Install the Dependencies

Run `bower install` to get all the dependencies.

### Viewing the Application

```
$ polymer serve
```

### Building the Application

```
$ polymer build
```

This will create a `build/` folder with `bundled/` and `unbundled/` sub-folders
containing a bundled (Vulcanized) and unbundled builds, both run through HTML,
CSS, and JS optimizers.

You can serve the built versions by giving `polymer serve` a folder to serve
from:

```
$ polymer serve build/bundled
```

### Running Tests

```
$ polymer test
```

The application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run the application's test suite locally.
