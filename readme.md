

# TACHYONS CUSTOM

You can find a generator for these themes at https://components.ai/tachyons-theme

Functional css for humans.

Quickly build and design new UI without writing css.

This is a fork of [Tachyons](https://github.com/tachyons-css/tachyons) with values being
configurable in a single variables file. More information about Tachyons can be found at http://tachyons.io

## Anithri's Fork
I like to use tachyons variables and default settings, while not using most of the tachyon's classes.  This fork is an 
edit of the tachyons source to remove all the classes I don't use.

Much of the media functionality is lost, but I don't use it anyway.

##### src/_variables.css
```
/*

    VARIABLES   

*/

@custom-media --breakpoint-not-small screen and (min-width: 30em);
@custom-media --breakpoint-medium screen and (min-width: 30em) and (max-width: 60em);
@custom-media --breakpoint-large screen and (min-width: 60em);

:root {
  --sans-serif: -apple-system, BlinkMacSystemFont, -system-ui, 'avenir next', avenir, helvetica, 'helvetica neue', ubuntu, roboto, noto, 'segoe ui', arial, sans-serif;
  --serif: athelas, serif;
  --monospace: SFMono, consolas, monaco, monospace;

  --font-size-headline: 6rem;
  --font-size-subheadline: 5rem;
  --font-size-1: 3rem;
  --font-size-2: 2.25rem;
  --font-size-3: 1.5rem;
  --font-size-4: 1.25rem;
  --font-size-5: 1rem;
  --font-size-6: 0.875rem;
  --font-size-7: 0.75rem;

  --measure: 30em;
  --measure-narrow: 20em;
  --measure-wide: 34em;

  --letter-spacing-tight:-.05em;
  --letter-spacing-1:.1em;
  --letter-spacing-2:.25em;

  --line-height-solid: 1;
  --line-height-title: 1.25;
  --line-height-copy: 1.5;

  --spacing-extra-small: 0.25rem;
  --spacing-small: 0.5rem;
  --spacing-medium: 1rem;
  --spacing-large: 2rem;
  --spacing-extra-large: 4rem;
  --spacing-extra-extra-large: 8rem;
  --spacing-extra-extra-extra-large: 16rem;

  --border-radius-1: 0.125rem;
  --border-radius-2: 0.25rem;
  --border-radius-3: 0.5rem;
  --border-radius-4: 1rem;
  --border-radius-circle: 100%;
  --border-radius-pill: 9999px;

  --box-shadow-1: 0px 0px 4px 2px rgba( 0, 0, 0, 0.2 );
  --box-shadow-2: 0px 0px 8px 2px rgba( 0, 0, 0, 0.2 );
  --box-shadow-3: 2px 2px 4px 2px rgba( 0, 0, 0, 0.2 );
  --box-shadow-4: 2px 2px 8px 0px rgba( 0, 0, 0, 0.2 );
  --box-shadow-5: 4px 4px 8px 0px rgba( 0, 0, 0, 0.2 );

  --height-1: 1rem;
  --height-2: 2rem;
  --height-3: 4rem;
  --height-4: 8rem;
  --height-5: 16rem;
  --width-1: 1rem;
  --width-2: 2rem;
  --width-3: 4rem;
  --width-4: 8rem;
  --width-5: 16rem;

  --max-width-1: 1rem;
  --max-width-2: 2rem;
  --max-width-3: 4rem;
  --max-width-4: 8rem;
  --max-width-5: 16rem;
  --max-width-6: 32rem;
  --max-width-7: 48rem;
  --max-width-8: 64rem;
  --max-width-9: 96rem;

  --red-000: #2a1311;
  --red-100: #4d1d1c;
  --red-200: #732627;
  --red-300: #9b2e32;
  --red-400: #c5363d;
  --red-500: #d95857;
  --red-600: #e57c76;
  --red-700: #f09d97;
  --red-800: #f8beb8;
  --red-900: #fddedb;
  --gold-000: #271609;
  --gold-100: #45240f;
  --gold-200: #663212;
  --gold-300: #894213;
  --gold-400: #ad5112;
  --gold-500: #d36110;
  --gold-600: #e48043;
  --gold-700: #f0a071;
  --gold-800: #f9bf9f;
  --gold-900: #ffdfce;
  --green-000: #111c0f;
  --green-100: #193218;
  --green-200: #1f4920;
  --green-300: #246227;
  --green-400: #287b2f;
  --green-500: #2b9637;
  --green-600: #2db13e;
  --green-700: #2dcd46;
  --green-800: #2cea4e;
  --green-900: #96fc93;
  --teal-000: #121b1b;
  --teal-100: #1b302f;
  --teal-200: #234644;
  --teal-300: #2b5e5a;
  --teal-400: #337672;
  --teal-500: #3a8f8a;
  --teal-600: #41aaa3;
  --teal-700: #48c4bd;
  --teal-800: #54e0d8;
  --teal-900: #b5f0eb;
  --blue-000: #131a26;
  --blue-100: #1c2d47;
  --blue-200: #22416b;
  --blue-300: #255791;
  --blue-400: #256db9;
  --blue-500: #4884d2;
  --blue-600: #769bdb;
  --blue-700: #9bb3e5;
  --blue-800: #bdccee;
  --blue-900: #dee5f6;
  --indigo-000: #201237;
  --indigo-100: #35196c;
  --indigo-200: #491fa7;
  --indigo-300: #5d22e6;
  --indigo-400: #7d41f8;
  --indigo-500: #9962fa;
  --indigo-600: #b282fc;
  --indigo-700: #c8a1fe;
  --indigo-800: #dcc0ff;
  --indigo-900: #eedfff;
  --violet-000: #2a121d;
  --violet-100: #4e1933;
  --violet-200: #761c4b;
  --violet-300: #9f1d65;
  --violet-400: #cb187f;
  --violet-500: #dd4a95;
  --violet-600: #e873a9;
  --violet-700: #f098be;
  --violet-800: #f7bbd3;
  --violet-900: #fcdde9;
  --gray-000: #191a1a;
  --gray-100: #2c2d2d;
  --gray-200: #3f4141;
  --gray-300: #545657;
  --gray-400: #696c6d;
  --gray-500: #808385;
  --gray-600: #979b9d;
  --gray-700: #b0b3b4;
  --gray-800: #cacccd;
  --gray-900: #e4e5e6;
}
```

## Getting started

Docs can be found at http://tachyons.io/docs
The modules are generally pretty small and thus easy to read and grock if you're familiar with css at all.

### Use the CDN

The quickest and easiest way to start using tachyons is to include a reference
to the minified file in the head of your html file.

Currently the latest version is 4.9.0
```html
<link rel="stylesheet" href="https://unpkg.com/tachyons@4.9.0/css/tachyons.min.css">
```

You can always grab the latest version with
```html
<link rel="stylesheet" href="https://unpkg.com/tachyons/css/tachyons.min.css">
```

### Local Setup

Clone the repo from github and install dependencies through npm.

```
git clone https://github.com/tachyons-css/tachyons-custom.git
cd tachyons-custom
npm install
```

#### Build

If you want to just use src as a jumping off point and edit all the code yourself, you can compile all of your wonderful changes by running

```npm start```

This will output both minified and unminified versions of the css to the css directory.

If you want to recompile everything from src everytime you save a change - you can run the following command, which will compile and minify the css

```npm run build:watch```

If you want to check that a class hasn't been redefined or 'mutated' there is a linter to check that all of the classes have only been defined once. This can be useful if you are using another library or have written some of your own css and want to make sure there are no naming collisions. To do this run the command

```npm run mutations```

## Contributing

If you want to make a PR to change part of the css source for tachyons, make sure you make the PR on the corresponding module
that can be found in the [tachyons org](http://github.com/tachyons-css/). Those modules get copied into the main repo so
any changes you make to the css in this repo would get overridden.

Also please read our [code of conduct](https://github.com/tachyons-css/tachyons/blob/master/code-of-conduct.md) for contributors.

## Websites that Use Tachyons
If you have a project or site that uses Tachyons feel free to make a PR to the (main repo) to add it to the list.

https://github.com/tachyons-css/tachyons/blob/master/sites.md



## Help

If you have a question feel free to open an issue here or jump into the [Tachyons slack channel](http://tachyons-slack-invite.herokuapp.com).

## License

MIT
