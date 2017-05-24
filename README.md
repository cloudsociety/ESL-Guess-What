# story-words

> A Vue-based *YES/NO* guessing game for ESL learners

One ESL learner thinks of an image and can only answer *yes* or *no*. Other learners ask *yes/no* questions to reduce the options to one. Avoid asking "Is it a [cat]". **Works great on interactive whiteboards.**

## How to use

After adding images and building the app, open `index.html`. Images can be toggled on or off until one remains. Refresh the window for new random board.

## Ideas
 * Has it got [4 legs]?
 * Is it [tall, red, hairy]?
 * Can it [run, swim, fly, eat meat]?
 * Does it [live in the sea]?

## Build Setup

``` bash
# install dependencies
npm install

# Add some images to the `images` folder. (sample images from placehold.it)
# each folder of images will be a single random image.
# filenames are not used and can be anything
npm run imgjson

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build
```
