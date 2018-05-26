# NPM-Workflow

Workflow using npm scripts, no gulp.

## Installation

```sh
$ git clone git@github.com:Divosky/NPM-Workflow.git
$ npm install
```

### Optionally

- Open `package.json` file and edit 7th line. Edit `--proxy` to change your server's name and `--startPath` to change website's directory.

### Commands

|      Command       | Result |
:-----------------: | ------------------------------------------------------------------------------
      `serve`       | Browser synchronization + run a server
  `autoprefixer`    | Run autoprefixer
`autoprefixer-dist` | Run autoprefixer and copy files into /dist (distribution) directory
      `scss`        | Compile scss to pure css
    `scss-dist`     | Compile scss to pure css and copy files into /dist (distribution) directory
      `lint`        | Check your js code (just in js folder)
     `uglify`       | Uglify js code and copy files into /dist (distribution) directory
    `build:css`     | Run `scss` and `autoprefixer`
 `build:css-dist`   | Run `scss-dev` and `autoprefixer-dev`
    `build:js`      | Run `lint`
  `build:js-dist`   | Run `lint` and `uglify`
   `build:html`     | Minify html files and copy files into /dist (distribution) directory
    `imagemin`      | Optimize images
  `imagemin-dist`   | Optimize images and copy files into /dist (distribution) directory
      `icons`       | Create sprite with icons
   `icons-dist`     | Create sprite with icons and copy the file into /dist (distribution) directory
  `build:images`    | Run `imagemin` and `icons`
`build:images-dist` | Run `imagemin-dist` and `icons-dist`
    `build:all`     | Run `build:css`, `build:js` and `build:images`
 `build:all-dist`   | Run `build:css-dist`, `build:js-dist`, `build:html`, `build:images-dist`
   `watch:scss`     | Watch scss files if there are any changes and if so - run `build:css`
    `watch:js`      | Watch js files if there are any changes and if so - run `build:js`
  `watch:images`    | Watch images if there are any changes and if so - run `build:images`
    `watch:all`     | Run a server and watch all the files
   `postinstall`    | Run `build:all` and `watch:all`

## Tested

Tested on:
- npm version: 4.2.0
- node version: 7.5.0
- Linux Arch, Linux Mint
