# Heroku buildpack: Meteor 0.9.2.2

## Usage

Then `git push` to heroku as usual.

## NOTES

You need to set the `ROOT_URL` environment variable:

```bash
heroku config:add ROOT_URL=http://your.domain.com
```

You can specify meteor settings by setting the `METEOR_SETTINGS` environment variable:

```bash
heroku config:add METEOR_SETTINGS='{"herp":"derp"}'
```
You need to have a verified account so the buildpack can add a `mongohq:sandbox` addon.

## Websockets

To enable websockets on Heroku, you will need to enable the "labs" feature:

```heroku labs:enable websockets```
