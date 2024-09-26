# Docs

## 🚀 Project Structure

```
/
├── public/
│   └──images/
├── pages/
│   ├──api/
│   │  └── health.ts
│   ├──*.{md,mdx}
│   ├──_meta.json
│   └── index.mdx
└── package.json
```

## 🧞 Commands

| Command          | Action                                         |
| :--------------- | :--------------------------------------------- |
| `npm install`    | Installs dependencies                          |
| `npm dev`        | Starts local dev server at `localhost:3000`    |
| `npm build`      | Build your production site to `./.next/`       |
| `npm preview`    | Preview your build locally, before deploying   |


## 🎉 Best Practices

- Use kebab case for folders (these will be the URLs in the doc site)
- Use relative links when linking within docs to prevent opening in a new tab

## 🗂️ Indexing folders

This allows for us to navigate to the upper level folder as a URL

- Add an index.mdx file for the folder
- In `pages/_meta.tsx`, add page index (should match folder name)
- To not have the index show up in the sidebar, add a `_meta.tsx` file in the folder with:

```jsx
export default {
  index: {
    display: "hidden",
  },
};
```





