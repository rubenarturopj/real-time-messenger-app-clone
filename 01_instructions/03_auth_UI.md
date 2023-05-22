# Auth UI

1. Create a folder called `components` in the `app/(site)/` folder. Insider create a file called `AuthForm.tsx` in `app/(site)/components` folder and export it as a`<AuthForm/>` component. Give it the basic structure. Mark it as `"use client"`.

2. In `app/(site)/page.tsx` place the `<AuthForm>` componente we just created. Don't forget to import it.

3. Go back to `AuthForm.tsx` to write it and style it.

-   Install react-icons, react-hook-form, clsx

```sh
npm install react-icons react-hook-form clsx
```

We are going to create a useState called `Variant`. Then we're going to add a type for this Variant that can be only or `"LOGIN"` or `"REGISTER"`; nothing else. And we're gonna pass it to the `useState` inside this signs `<>.` Like this: `useState<Variant>`.

Create a toglle function to control if we are login in or registering.

Below create a useForm and pass it the FieldValues.

Style the return section, here special attention to the `onSubmit` property of the `form`. Which will be `handleSubmit(onSubmit)`. `HandleSubmit` comes from `react-hook-form` and inside of it goes the `obSubmit` we created ouserselves. If we don't use `handleSubmit` then we can't get the `data` for the other function.

Later we'll need an `<input>` component that we are going to create in the next step.

4. go to `app/` folder and create a new folder called `component`. This component folder is NOT tight to the router (app/(site)/stuff) but this will be totally independant. Inside this new component folder, create a new folder called `input`. Inside it create the `input.tsx` file and pass it in the returning section of the `AuthForm.tsx` file. Don't forget to add "use client" to this input.

In this `Input.tsx` file, we are going to import `clsx` that we installed before. Also, import the variables `react-hook-form`.

Create an interface for this file.

5. Install `TailWind CSS form`. Stop the app first.

```sh
npm i @tailwindcss/forms
```

Then go to `tailwind.config.js` and in `plugins` write `require("@tailwindcss/forms")({strategy: "class"})`.

Run the app again.

6. Go back to the `input` component. And keep working in the return.

7. Once done go back to `AuthForm.tsx` and make the input to render conditionally. Change the id and label to name. Then Write more Inputs below. Keep styling. We will need a `<button>` and a `<AuthSocialButton>` compontents

8. Create the `<button>` component in a file named `Button.tsx` in the `app/components` folder (not the site one). Fill it and style it. Create an interface as well. This component will have `{children}` inside the tags. So it takes inside the button whatever we put between the tags in the other place where it is used.

9. Create the `<AuthSocialButton>` component in a file named: `AuthSocialButton.tsx` in the `app/(site)/components` folder (not the folder for the independant components.). And write it
