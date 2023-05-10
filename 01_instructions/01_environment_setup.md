# Create app

1. In the terminal run:

```sh
npx create-next-app@latest --typescript --tailwind
```

In the prompt choose:

| asked                      | choose |
| -------------------------- | ------ |
| ok to proceed?             | yes    |
| ESlint                     | yes    |
| src/directory              | no     |
| app router / app directory | yes    |
| alias                      | no     |

2. run your app and go to `localhost:3000` to see it.

```sh
npm run dev
```

3. Go to `app/page.tsx` and remove everything except the return function. Write a temporary div in the meantime.

4. Go to `app/layout.tsx` and you can change the name of the website if you want to.

5. Go to `global.css` and delete everything, except the `tailwind` directs on top. Also write this below:

```sh
html,
body,
:root {
  height: 100%;
}
```

6. Go to `tailwind.config.js` and delete everything inside the `extend` section.
