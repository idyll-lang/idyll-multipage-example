# idyll-multipage-example
Example repo for setting up an Idyll blog with multiple posts.

### Project overview

- `posts` - all of the available posts, each directory within contains a full idyll post
- `components` - shared components, can be used by any post. Each post also has its own component's folder where you can put components that don't need to be shared.
- `template` - the post template to use when you run `idyll create`.
- `public` - the folder where the output is built. You can deploy this to any static hosting service.

## Installation

- Make sure you have `idyll` installed (`npm i -g idyll`).
- Clone this repo and run `npm install`.

## Creating a post

Navigate to the posts directory and run `idyll create --template ../template/`

## Developing a post locally

Navigate to the post's directory and run `idyll`.

## Building a post for production

Navigate to the post's directory and run `idyll build`. The output will appear in the top-level `public` folder.

## Deploying

Make sure all of your posts have been built, then deploy the public folder via any static hosting service.


# Known limitations

- Note that idyll.pub (used by the `idyll publish` command) does not yet support multi-page projects such as this one, so it is up to you host the output online.