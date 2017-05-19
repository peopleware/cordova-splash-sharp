# cordova-splash-sharp

Automatic splash screen generator for Cordova. Create a splash screen (2208x2208) once in the root folder of your Cordova project and use cordova-splash-sharp to automatically crop and copy it for all the platforms your project supports (currenty works with iOS, Android and Windows 10).

### Installation

    $ sudo npm install cordova-splash-sharp -g

### Requirements

- At least one platform was added to your project ([cordova platforms docs](http://cordova.apache.org/docs/en/edge/guide_platforms_index.md.html#Platform%20Guides))
- Cordova's config.xml file must exist in the root folder ([cordova config.xml docs](http://cordova.apache.org/docs/en/edge/config_ref_index.md.html#The%20config.xml%20File))

### Usage

Create a `splash.png` file in the root folder of your cordova project and run:

    $ cordova-splash-sharp

You also can specify manually a location for your `config.xml` or `splash.png`:

    $ cordova-splash-sharp --config=config.xml --splash=splash.png

If you run a old version of Cordova for iOS and you need your files in `/Resources/icons/`, use this option:

    $ cordova-splash-sharp --xcode-old

### Icons

Check out [cordova-icon](https://github.com/AlexDisler/cordova-icon)

### License

MIT
