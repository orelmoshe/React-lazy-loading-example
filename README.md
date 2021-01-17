# What is React.lazy()

It is a new function in react that lets you load react components lazily through code splitting without help from any additional libraries. Lazy loading is the technique of rendering only-needed or critical user interface items first, then quietly unrolling the non-critical items later. It is now fully integrated into core react library itself. We formerly used react-loadable to achieve this but now we have react.lazy() in react core.

---

# Suspense

Suspense is a component required by the lazy function basically used to wrap lazy components. Multiple lazy components can be wrapped with the suspense component. It takes a fallback property that accepts the react elements you want to render as the lazy component is being loaded.

---

# Why is Lazy Loading (& Suspense) Important

Firstly, bundling involves aligning our code components in progression and putting them in one javascript chunk that it passes to the browser; but as our application grows, we notice that bundle gets very cumbersome in size. This can quickly make using your application very hard and especially slow. With Code splitting, the bundle can be split to smaller chunks where the most important chunk can be loaded first and then every other secondary one lazily loaded.

Also, while building applications we know that as a best practise consideration should be made for users using mobile internet data and others with really slow internet connections. We the developers should always be able to control the user experience even during a suspense period when resources are being loaded to the DOM.

---

### project overview:

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

I'm showcasing a bunch of videos in both desktop & mobile layout

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.
