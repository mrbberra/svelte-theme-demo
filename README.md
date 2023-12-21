# Demo app to show how themes might work

Important files:

- `src/routes/layout.svelte`: sets theme class on document root element. Not the cleanest thing, but svelte doesn't support anything better right now (see this [GH issue](https://github.com/sveltejs/svelte/issues/3105)). It's pulling from the store, because I imagine that when this is actually implemented, we will want to decide the theme based on information (user grade level) from the store.
- `themes.scss` defines the custom css variables for the themes.

## Testing it out

```
npm install
```

And then:

```
npm run build
npm run preview
```

For some reason, `npm run dev` doesn't get the styles showing up correctly.
