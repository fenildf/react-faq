# React FAQ

This guide aims to pull together quality content about React core concepts into a central location for quick reference.

Remember we're all learning.  Read, Try, Mess Up (it's okay).

### Other Languages
[🇪🇸 Español](https://github.com/xDae/react-faq)  
[🇨🇳 简体中文](https://github.com/justjavac/react-faq)

#Start
>There's lots to learn but if you break it down there are some key concepts to focus on. JSX, React elements, Components, Lifecycle Methods, Props and State.  These articles will start you down the path to learning React.

**I don't know React what should I watch / read before I start?**
* [Thinking in React - Pete Hunt](https://facebook.github.io/react/docs/thinking-in-react.html)
* 🔥 [Teaching React Without Using React](https://medium.com/@ericclemmons/teaching-react-without-using-react-a4b87cfd4e87#.q8cyvryw1) Eric Clemmons @ericclemmons
* 🔥 [13 things you need to know about React](http://aimforsimplicity.com/post/13-things-you-need-to-know-about-react)  @kjendrzyca
* [The 5 Things You Need To Know To Understand React](https://medium.com/@sachagreif/the-5-things-you-need-to-know-to-understand-react-a1dbd5d114a3#.uii8of7um) Sacha Greif

**Official React Docs are a great resource**
* [Official React Docs](https://facebook.github.io/react/docs/hello-world.html)

**Additional information to start with**
* [Pete Hunt: React: Rethinking best practices (JSConf EU 2013)](https://www.youtube.com/watch?v=x7cQ3mrcKaY)
* [React in 7 Minutes](https://egghead.io/lessons/react-react-in-7-minutes) this is a slightly dated but still really good starter
* [Complete Intro to React - React, Webpack, Babel, Redux, React Router, SSR](https://btholt.github.io/complete-intro-to-react/) Brian Holt(@holtbt) for Frontend Masters worshop
* [React "Aha" Moments](https://tylermcginnis.com/react-aha-moments) Tyler McGinnis @tylermcginnis33
* [All the terrible things I did the first time I wrote a complex React App ](https://youtu.be/Fk--XUEorvc?t=20666) Raquel @raquelxmoss
* [Introduction to React](https://mva.microsoft.com/en-US/training-courses/introduction-to-react-16635?l=4wrKgdJrC_206218965) Eric W. Greene / Microsoft Virtual Academy

## Resources

- [History](#history)
- [Creating a React Project](#creating-a-react-project)
- [Why use React?](#why-use-react)
- [JSX](#jsx)
- [The Virtual DOM](#the-virtual-dom)
- [React elements](#react-elements)
- [Components](#components)
  - [Lifecycle Methods](#lifecycle-methods)
  - [Component Types](#component-types)
  - [Finding Components](#finding-components)
  - [Controlled Components](#controlled-components)
  - [Props](#props)
  - [PropTypes](#proptypes)
  - [State](#state)
  - [Children API](#children-api)
  - [Binding](#binding)
  - [Events](#events)
  - [Rendering](#rendering)
  - [Keys](#keys)
  - [Refs](#refs)
- [Context](#context)
- [Forms](#forms)
- [React Ajax](#react-ajax)
- [Patterns](#patterns)
- [Gotchas](#gotchas)
- [PATENTS](#patents)
- [Internationalization](#internationalization)
- [Third Party Libraries](#third-party-libraries)
- [Performance](#performance)
- [Animations](animations.md)
- [SVG & React](#svg--react)
- [React Style Guides](#react-style-guides)
- [Redux and Mobx](#redux-and-mobx)
- [Adding React to an existing app](#adding-react-to-an-existing-app)
- [CSS and React](css.md)
- [Testing](testing.md)
- [Deep Dive](deep-dive.md)
- [React Fiber](react-fiber.md)
- [Video Courses](videos-courses.md)
- [A11Y](a11y.md)
- [Talks](talks.md)
- [Training](training.md)
- [Books](books.md)
- [Newsletters](newsletters.md)
- [Interview Questions](interview-questions.md)
- [Tools](tools.md)
- [Server-Side Rendering](server-side-rendering.md)


#History
* [JSConfUS 2013 - Tom Occhino and Jordan Walke: JS Apps at Facebook](https://www.youtube.com/watch?v=GW0rj4sNH2w&index=10&list=PL37ZVnwpeshF7AHpbZt33aW0brYJyNftx) The one where React became #OSS
* [Our First 50,000 Stars](https://facebook.github.io/react/blog/2016/09/28/our-first-50000-stars.html) Vjeux @vjeux

#Creating a React Project

**How do I create a new React project?**

> That depends on what your looking for out of the box.  No config, config, server-rendered etc... here are a few to consider.  Of course you can setup from scratch as well (not covered here).

* [create-react-app](https://github.com/facebookincubator/create-react-app) No configuration or complicated folder structures, just the files you need to build your app.
* [nwb](https://github.com/insin/nwb) Create React apps with no configuration (until you need it)
* [next.js](https://github.com/zeit/next.js) A minimalistic framework for universal server-rendered React applications
* [react-server](https://github.com/redfin/react-server) Batteries-included Server-rendered React applications. Note: also see [React 30 -> 002 - Streaming React](https://www.youtube.com/watch?v=XW_c60NCkI4)
* [react-boilerplate](https://github.com/mxstbr/react-boilerplate) A highly scalable, offline-first foundation with the best DX and a focus on performance and best practices
* [create-react-pwa](https://github.com/jeffposnick/create-react-pwa create-react-app) + Progressive Web App goodness
* [gatsby](https://github.com/gatsbyjs/gatsby) Transform plain text into dynamic blogs and websites using React.js

Also see these [projects](https://github.com/facebookincubator/create-react-app#alternatives)


**Where can I find videos for using React Create App?**

[React Create App + Express](https://www.youtube.com/watch?v=gbVhmaW04bc&feature=youtu.be) @sprjrx @ladyleet


**Can I play around with React Online?**

* [extends React.Component style](http://codepen.io/Arney/pen/OXYqWb)
* [React.createClass style](http://codepen.io/Arney/pen/QERoaQ)
* [React JSBin](http://react.jsbin.com/?html,css,js,output)
* [WebpackBin](http://www.webpackbin.com/EkscblgMM)

#Why use React?

>
* Composable components
* Easy to use with existing projects
* Declarative
* Functional / Immutable friendly


**Is it fast?**
* [Is React.js fast? Faster than {framework}? … or are there more relevant questions to be asking?](https://medium.com/react-weekly/is-react-js-fast-faster-than-framework-or-are-there-more-relevant-questions-to-be-asking-bcf40211f89b#.ll2aubhbi) Jeff Barczewski @jeffbski

**What so good about React?**

* [7 Strengths of React Every Programmer Should Know About](https://vacuumlabs.com/blog/7-strengths-of-react-every-programmer-should-know-about) Samuel Hapák @samuha
* [Design Principles](https://facebook.github.io/react/contributing/design-principles.html)

#JSX
**What's JSX?**

>JSX is a preprocessor step that adds XML syntax to JavaScript. You can definitely use React without JSX but JSX makes React a lot more elegant. - http://buildwithreact.com

* [Tutorial: JSX](http://buildwithreact.com/tutorial/jsx)
* [JSX in Depth](https://facebook.github.io/react/docs/jsx-in-depth.html)
* [React’s JSX: The Other Side of the Coin](https://medium.com/@housecor/react-s-jsx-the-other-side-of-the-coin-2ace7ab62b98#.i5rmd9h07) Cory House @housecor
* [What does JSX stand for?](https://twitter.com/tomocchino/status/769931611303321601) Tom Occhino @tomocchino

**What does JSX really do for me?**

[This is the sort of stuff JSX saves you from having to manage](https://gist.github.com/insin/8e72bed793772d82ca8d) Jonny Buchanan @jbscript

#The Virtual DOM

>The Virtual DOM provides a lightweight implementation of the DOM and events system. Instead of dealing with the browser, you manipulate an in-memory version of the DOM.

**What is the Virtual DOM?**
* 💯  [The Inner Workings Of Virtual DOM](https://medium.com/@rajaraodv/the-inner-workings-of-virtual-dom-666ee7ad47cf#.q3jxayda5) @rajaraodv
* [React's diff algorithm](http://calendar.perfplanet.com/2013/diff/) Christopher Chedeau @vjeux
* [The one thing that no one properly explains about React — Why Virtual DOM](https://hashnode.com/post/the-one-thing-that-no-one-properly-explains-about-react-why-virtual-dom-cisczhfj41bmssp53mvfwmgrq) Sai Kishore Komanduri @saiki
* [Pete Hunt: The Secrets of React's Virtual DOM (FutureJS 2014)](https://www.youtube.com/watch?v=-DX3vJiqxm4)

**Is the Virtual DOM all about speed?**

*No*

See :

https://twitter.com/dan_abramov/status/790326092582252544
https://twitter.com/acdlite/status/779693791607336960

> I wonder if we can reclaim the VDOM term to mean "Value DOM", as in Value Type, instead of "Virtual DOM"...? More accurate. **@sebmarkbage**
<hr>
> It doesn't improve perf over hand written DOM code but it's hard to write on scale. React scales well. **@dan_abramov**
<hr>
> React ultimately has to call browser APIs at some point, it can't possibly be faster than writing the same exact calls by hand **@dan_abramov**
<hr>
>React will not do anything that you cannot. By definition everything it does can be reproduced (and some people have with other libraries/frameworks that follow similar conventions). The point is not that React does something that you can't, but rather that by introducing React to your application you are relieved of having to worry about manually handling your DOM, manually determining how to update it efficiently, minimizing traversals, etc. - [Sean Grogg](https://www.quora.com/Is-ReactJS-faster-than-direct-DOM-manipulation-with-JavaScript-or-jQuery)

**Key Takeaway:**

> React keeps your product reasonably fast without you having to think about it all the time, or to jump through the hoops **@dan_abramov**

#React elements
> Elements are the smallest building blocks of React apps.
> Elements are what components are "made of ..."
— [React Docs](https://facebook.github.io/react/docs/rendering-elements.html)

* [What makes an 'Element' an 'Element' vs a component?](https://twitter.com/timarney/status/790540834466701312) Tim Arney @timarney
* [Understanding the Difference Between React Elements and Components](https://quickleft.com/blog/understanding-the-difference-between-react-elements-and-components) Alex Johnson
* [React Elements vs React Components](https://tylermcginnis.com/react-elements-vs-react-components) Tyler McGinnis

#Components
> Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. Conceptually, components are like JavaScript functions. - [React Docs](https://facebook.github.io/react/docs/components-and-props.html)

**What are some of your best practices when working with components?**

> * Keep it (F)ocused.
* Keep it (I)ndependent.
* Keep it (R)eusable.
* Keep it (S)mall.
* Keep it (T)estable.
* or in short, `FIRST`.

> — Addy Osmani https://addyosmani.com/first

See :  https://twitter.com/mxstbr/status/790084862954864640 Max Stoiber @mxstbr

#Lifecycle Methods

>Components have several "lifecycle methods" that allow you to override / run code at particular times.

**What are Lifecycle Methods?**

* [React components lifecycle diagram](http://codepen.io/eduardoboucas/full/jqWbdb) Eduardo Bouças @eduardoboucas
* [React lifecycle cheatsheet](https://gist.github.com/bvaughn/923dffb2cd9504ee440791fade8db5f9) @brian_d_vaughn 
* [Going further with React lifecycle methods](https://medium.com/@notrab/going-further-with-react-lifecycle-methods-2ffdc5bdf52c#.bu0ufrosb) Jamie Barton
* [Component Specs and Lifecycle](https://facebook.github.io/react/docs/component-specs.html)
* [My #reactjs component lifecycle cheatsheet for quick reference](https://twitter.com/pbesh/status/738008776805060608) Peter Beshai @pbesh
* [React component’s lifecycle](https://medium.com/react-ecosystem/react-components-lifecycle-ce09239010df#.w7v5cw6tk) Osmel Mora @osmel_mora

#Component Types
> There are two main types of components Functional and Class Components

```
// Functional Component
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}

// Class Component

class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
```
Components can be used (composed) in many ways see the following links for patterns and thoughts on creating Components.

**How do I decide what type of Component to use?**

>This comes down to a few factors... a primary one being you need to decide what a component should do.  
See: [Some Thoughts on Function Components in React](https://medium.com/javascript-inside/some-thoughts-on-function-components-in-react-cb2938686bc7#.2oazdyli1) from A. Sharif @sharifsbeat for some help deciding.

<hr>

> In this video [React Component Patterns by Michael Chan](https://www.youtube.com/watch?v=YaZg8wg39QQ) @chantastic breaks down some of the component types in a less technical way (using circles).

Also:

* [React.Component vs React.createClass](https://reactjsnews.com/composing-components) Naman Goel & Zach Silveira
* [React.createClass versus extends React.Component](https://toddmotto.com/react-create-class-versus-component) Todd Motto
* [4 different kinds of React component styles](https://www.peterbe.com/plog/4-different-kinds-of-react-component-styles) Peter Bengtsson @peterbe
* [Functions as Child Components and Higher Order Components](http://rea.tech/functions-as-child-components-and-higher-order-components) Ken Ding

**Stateless Function** [```<Code />```](http://reactpatterns.com/#stateless-function)

* [React Stateless Functional Components: Nine Wins You Might Have Overlooked](https://medium.com/@housecor/react-stateless-functional-components-nine-wins-you-might-have-overlooked-997b0d933dbc#.iydj782xq) Cory House @housecor
* [Embracing Functions in React](https://medium.com/javascript-inside/embracing-functions-in-react-d7d558d8bd30#.igvxagy0e) A. Sharif @sharifsbeat

**Presentational and Container Components**  [```<Code />```](http://reactpatterns.com/#container-component)

* [Presentational and Container Components](https://medium.com/@dan_abramov/smart-and-dumb-components-7ca2f9a7c7d0#.xo2al5187) Dan Abramov @dan_abramov

**Higher-Order Components** [```<Code />```](http://reactpatterns.com/#higher-order-component)

* [ReactCasts #1 - Higher Order Components](https://www.youtube.com/watch?v=LTunyI2Oyzw) Cassio Zen @cassiozen
* [React Higher Order Components in depth](https://medium.com/@franleplant/react-higher-order-components-in-depth-cf9032ee6c3e#.mpb29ree6) @franleplant
* [Higher Order Components: A React Application Design Pattern](https://www.sitepoint.com/react-higher-order-components) Jack Franklin @Jack_Franklin
* [Mixins Are Dead. Long Live Composition](https://medium.com/@dan_abramov/mixins-are-dead-long-live-higher-order-components-94a0d2f9e750#.prpfdo79n) Dan Abramov @dan_abramov
* [Higher Order Components: Theory and Practice](http://engineering.blogfoster.com/higher-order-components-theory-and-practice)
* [Real World Examples of Higher-Order Components](http://rea.tech/reactjs-real-world-examples-of-higher-order-components/) Mehdi Mollaverdi @mehdimollaverdi
* [Start Reacting: HOC](https://www.youtube.com/watch?v=ymJOm5jY1tQ) OliverFencott @OliverFencott

**Function as Child Components** [```<Code />```](http://reactpatterns.com/#function-as-children)

* [ReactCasts #2 - Function as Child Components](https://www.youtube.com/watch?v=WE3XAt9P8Ek) Cassio Zen @cassiozen
* [Function as Child Components](https://medium.com/merrickchristensen/function-as-child-components-5f3920a9ace9#.10fbiyqc5) Merrick Christensen @iammerrick
* [I've mentioned this before, but I'm a big fan of child functions in React](https://twitter.com/brian_d_vaughn/status/779362701596164097) Brian Vaughn @brian_d_vaughn

**What types of components are there?**

* [React Component Jargon as of August 2016](https://blog.anthonycomito.com/react-component-jargon-as-of-august-2016-28451d8ceb1d#.a417p5u26) Anthony Comito @a_comito

#Finding Components

**Where are some good places to find components?**

* [React Components Catalog](https://github.com/brillout/awesome-react-components)
* [React Rocks](https://react.rocks)

#Controlled Components

**What is a controlled component?**

Via Loren Stewart @lorenstewart111 [React.js Forms: Controlled Components](http://lorenstewart.me/2016/10/31/react-js-forms-controlled-components)

>A controlled component has two aspects:

1. Controlled components have functions to govern the data going into them on every onChange event, rather than grabbing the data only once, e.g. when a user clicks a submit button. This 'governed' data is then saved to state (in this case, the parent/container component's state).

2. Data displayed by a controlled component is received through props passed down from it's parent/container component.

> This is a one-way loop – from (1) child component input (2) to parent component state and (3) back down to the child component via props – is what is meant by unidirectional data flow in React.js application architecture.

#Props

**What are props?**
>props (short for properties) are a Component's configuration, its options if you may. They are received from above and immutable as far as the Component receiving them is concerned. - react-guide

See : [props vs state](https://github.com/uberVU/react-guide/blob/master/props-vs-state.md)

**How do I pass props?**

* [Transferring Props](https://facebook.github.io/react/docs/transferring-props.html)

**How do I pass boolean values?**

* [JSX `<Foo bar={true} />` and `<Foo bar>` are equivalent](https://twitter.com/Jack_Franklin/status/768735664485568512) Jack Franklin @Jack_Franklin

**Should I use import, props, or context in React?**

* [Differences between require() and passing an object via prop or context](http://stackoverflow.com/questions/39111775/differences-between-require-and-passing-an-object-via-prop-or-context/39111942) Dan Abramov @dan_abramov

#PropTypes

>PropTypes are essentially a dictionary where you define what props your component needs and what type(s) they should be. -  Niels Gerritsen

**What are PropTypes?**
* [What are PropTypes?](https://themeteorchef.com/snippets/what-are-proptypes) Ryan Glover @themeteorchef

**Why are React PropTypes important?**
* [Why React PropTypes are important](http://wecodetheweb.com/2015/06/02/why-react-proptypes-are-important)  Niels Gerritsen @NielsG89

**How do I validate props?**
* [Better Prop Validation in React](https://medium.com/@MoeSattler/better-prop-validation-in-react-cc83590d311f#.wdhbsrlgj) Moe Sattler @travelperk

#State

> In one sense, “state” means the current visual representation of the app on screen... In the React sense, “state” is an object that represents the parts of the app that can change. Each component can maintain its own state, which lives in an object called this.state. - Dave Ceddia

**What is state in React?**

* [A Visual Guide to State in React](https://daveceddia.com/visual-guide-to-state-in-react) Dave Ceddia @dceddia

**How do I handle state?**

* [The 5 Types Of React Application State](http://jamesknelson.com/5-types-react-application-state) James K Nelson @james_k_nelson
* [State of React #1: A Stateless React App?](http://jamesknelson.com/state-react-1-stateless-react-app) James K Nelson @james_k_nelson
* [A Case for setState](https://medium.com/@zackargyle/a-case-for-setstate-1f1c47cd3f73#.w89epdtmo) Zack Argyle
* [Where to Hold React Component Data: state, store, static, and this](https://medium.freecodecamp.com/where-do-i-belong-a-guide-to-saving-react-component-data-in-state-store-static-and-this-c49b335e2a00#.8k7tc37cs) Sam Corcos
* [How to handle state in React. The missing FAQ](https://medium.com/react-ecosystem/how-to-handle-state-in-react-6f2d3cd73a0c#.dwz84fx9s) Osmel Mora @osmel_mora
* [Should I keep something in React component state? I made a small cheatsheet.](https://twitter.com/dan_abramov/status/749710501916139520) Dan Abramov @dan_abramov
* [Best Practices for Component State in React.js](http://brewhouse.io/blog/2015/03/24/best-practices-for-component-state-in-reactjs.html) Gabe Scholz @gabescholz
* [Exploring React’s State Propagation](https://www.sitepoint.com/exploring-reacts-state-propagation) Eric Greene @ericwgreene

**How can I decouple state and UI?**

* [How to decouple state and UI](https://medium.com/@mweststrate/how-to-decouple-state-and-ui-a-k-a-you-dont-need-componentwillmount-cc90b787aa37#.7l8ji1wer) Michel Weststrate @mweststrate


**Coming from jQuery... how do I adjust my mental modal to work with React / State?**
* [Thinking Statefully](https://daveceddia.com/thinking-statefully) Dave Ceddia @dceddia

**I heard you can pass a function to setState when should do that?**
* [Using a function in `setState` instead of an object](https://medium.com/@shopsifter/using-a-function-in-setstate-instead-of-an-object-1f5cfd6e55d1#.h3fokbh9a) Sophia Shoemaker

#Children API

* [ReactCasts #3 - React's Children API](https://www.youtube.com/watch?v=DJ53-G8EbxE) Cassio Zen @cassiozen
* [A deep dive into children in React](https://mxstbr.blog/2017/02/react-children-deepdive) Max Stoiber @mxstbr

#Binding
>The JavaScript bind method has several uses. Typically, it is used to preserve execution context for a function that executes in another context.

<hr>
**How do I bind events (i.e. onClick) in React?**
> There are several ways to bind things in React [this video](https://egghead.io/lessons/javascript-public-class-fields-with-react-components?pl=javascript-from-kent-ff87bbdb) via Kent C. Dodds + @eggheadio covers multiple ways to bind events showing the benefits and drawbacks for each.



**What should you use for binding methods in React classes?**
* [To bind or not to bind?](https://twitter.com/dan_abramov/status/790612782471319553) Dan Abramov @dan_abramov
* [fat Arrow vS Autobind VS bind](https://www.reddit.com/r/reactjs/comments/54xnao/fat_arrow_vs_autobind_vs_bindbindbindbindbind/d85wj0l) Dan Abramov @dan_abramov

**What is this bind thing?**

* [Don't Use Bind When Passing Props](https://daveceddia.com/avoid-bind-when-passing-props) Dave Ceddia
* [5 Approaches for Handling Binding](https://medium.com/@housecor/react-binding-patterns-5-approaches-for-handling-this-92c651b5af56#.4z71l0kmb) Cory House @housecor
* [How to Deal with `this` Reference Inside the Promise?](https://www.toptal.com/react/tips-and-practices) Toptal Developers

#Events

**How does the event system work in React?**

* [React events in depth](https://www.youtube.com/watch?v=dRo_egw7tBc) Kent C. Dodds, Ben Alpert, & Dan Abramov

#Rendering

**What should go in the render function?**

* [Return as soon as you know the answer](https://medium.com/@SimonRadionov/return-as-soon-as-you-know-the-answer-dec6369b9b67#.82kxymyki) @SimonRadionov

#Keys
>React uses [keys](https://facebook.github.io/react/docs/reconciliation.html#keys) to help with Reconciliation (i.e. how it calculates the DOM diff for each render).

```
<ul>
  <li key="2015">Duke</li>
  <li key="2016">Villanova</li>
</ul>
```

>  As noted in 'What should I use for a key?' Be careful what you use for a key.  Using an array index isn't a best practice... aim to use a unique id.

**Why can't i put key in default props (or define the default somewhere else)?**

* [Why can't i put key in default props](https://www.reddit.com/r/reactjs/comments/4mjdcf/why_cant_i_put_key_in_default_props_or_define_the/d3xwa6m)

**What should I use for a key?**

* [Index as a key is an anti-pattern](https://medium.com/@robinpokorny/index-as-a-key-is-an-anti-pattern-e0349aece318#.y4ru46ikc) Robin Pokorný @robinpokorny

**What are some examples where I should manually change a key?**

* [The key is using key](https://twitter.com/timarney/status/730785238654287873) Tim Arney @timarney

#Refs
>The ref attribute makes it possible to store a reference to a particular React element or component returned by the component render() configuration function. This can be valuable when you need a reference, from within a component, to some element or component contained within the render() function. - reactenlightenment.com

**What are refs and are string refs are bad?**

* [Refs to Components](https://facebook.github.io/react/docs/more-about-refs.html)
* [Why do you use findDOMNode()?](https://twitter.com/dan_abramov/status/752936646602031104) Dan Abramov @dan_abramov
* [String refs are bad in quite a few ways](https://news.ycombinator.com/edit?id=12093234) Dan Abramov @dan_abramov

#Context
⚠️ Context is an **advanced and experimental** feature. The API is likely to change in future releases. The rumours of its existence are true but be careful!

* [ReactCasts #4 - Context (Part 1)](https://www.youtube.com/watch?v=lxq938kqIss&t=1s) Cassio Zen @cassiozen
* [ReactCasts #5 - Context (Part 2)](https://www.youtube.com/watch?v=mwYHDXS6uSc&feature=youtu.be) Cassio Zen @cassiozen
* [How to handle React context in a reliable way](https://medium.com/react-ecosystem/how-to-handle-react-context-a7592dfdcbc#.rtwgxxy0d) Osmel Mora @osmel_mora
* [How to safely use React context](https://medium.com/@mweststrate/how-to-safely-use-react-context-b7e343eff076#.m6v9tsgub) Michel Weststrate @mweststrate
* [Context all the things with React](https://www.youtube.com/watch?v=k9AhBMwj1w4) Stephen Rivas Jr. (@sprjrx)

#Forms

**How can I build forms with React?**

* [Learn Raw React: Ridiculously Simple Forms](http://jamesknelson.com/learn-raw-react-ridiculously-simple-forms) James K Nelson @james_k_nelson

**How can I validate form input?**
* [Elegant Form Validation Using React](https://spin.atomicobject.com/2016/10/05/form-validation-react) Jordan Schaenzle
* [Building validated forms with great UX in React](https://youtu.be/1Urj4TZ5BLI?t=2437) Marcela Hrdá
* [react-validation](https://github.com/vacuumlabs/react-validation)


#React Ajax

**What is the best practice for getting server data into React components?**
>It depends! See: [React AJAX Best Practices](http://andrewhfarmer.com/react-ajax-best-practices) Andrew H Farmer @ahfarmer

* [Loading and Using External Data in React](http://mediatemple.net/blog/tips/loading-and-using-external-data-in-react) Chris Coyier @chriscoyier

#Patterns

* [React Patterns](http://reactpatterns.com) @chantastic
* [React.js in patterns](http://krasimirtsonev.com/blog/article/react-js-in-design-patterns) Krasimir Tsonev
* [Patterns For Style Composition In React](http://jxnblk.com/writing/posts/patterns-for-style-composition-in-react) Brent Jackson @jxnblk
* [Make Your React Components Pretty](https://medium.com/walmartlabs/make-your-react-components-pretty-a1ae4ec0f56e#.ctwfvx379) Mark Brouch @markbrouch

#Gotchas

**What are some React Gotchas?**

* [React Gotchas](https://daveceddia.com/react-gotchas) Dave Ceddia @dceddia 
* [How to Render Components Outside the Main ReactJS App](https://blog.komand.com/how-to-render-components-outside-the-main-react-app)
* [Watch Out for Undefined State](https://daveceddia.com/watch-out-for-undefined-state) Dave Ceddia @dceddia 

**How do you add comments in JSX?**

```
render() {
  return (
    <div>
      <!-- Fail -->
    </div>
  )
}

render() {
  return (
    <div>
      {/* Works! */}
    </div>
  )
}

```
More info and Sublime Text snippet here: http://wesbos.com/react-jsx-comments @wesbos

#PATENTS

**What's all this stuff I hear about Facebook PATENTS clause?**

* [Some links to point people to when they misinterpret PATENTS clause or spread false claims](https://gist.github.com/gaearon/df0c4025e67399af72786d7ac7c819cc) Dan Abramov @dan_abramov
* [React’s license: necessary and open?](http://lu.is/blog/2016/10/31/reacts-license-necessary-and-open) Luis Villa @luis_in_140

#Internationalization

**How should I handle internationalization?**

* [Internationalization in React](https://medium.freecodecamp.com/internationalization-in-react-7264738274a0#.bcfxgycwv) Preethi Kasireddy

**What repos should I checkout for internationalization?**
* [react-intl](https://github.com/yahoo/react-intl)
* [react-localize](https://github.com/sprjr/react-localize) @sprjrx

#Third Party Libraries

**How do I use third party libraries?**

* [Integration with Third Party Libraries](https://www.youtube.com/watch?v=GWVjMHDKSfU&feature=youtu.be&a) Rally Coding

#Performance

**How can I make my app faster?**

* [Component Rendering Performance in React](https://medium.com/modus-create-front-end-development/component-rendering-performance-in-react-df859b474adc#.gvyat7vkb) Grgur Grisogono
* [Don‘t use PureComponent everywhere. Measure](https://twitter.com/dan_abramov/status/759383530120110080) Dan Abramov @dan_abramov
* [React.js pure render performance anti-pattern](https://medium.com/@esamatti/react-js-pure-render-performance-anti-pattern-fb88c101332f#.hewsz120q)
* [Should I use shouldComponentUpdate?](http://jamesknelson.com/should-i-use-shouldcomponentupdate) James K Nelson @james_k_nelson
* [Reconciliation](https://facebook.github.io/react/docs/reconciliation.html)
* [Quick slides on #reactjs performance](http://presentations.survivejs.com/react-performance/#/?_k=ivqhoe) Juho Vepsäläinen @bebraw

#SVG & React

**How do I work with SVG's in React?**

* [Icons as React Components](https://medium.com/@david.gilbertson/icons-as-react-components-de3e33cb8792#.lmbz3v9ic)
* [Creating an SVG Icon System with React](https://css-tricks.com/creating-svg-icon-system-react) @sarah_edo

#React Style Guides

**Where can I find some good React  style guides?**

* [Eventbrite React & JSX Coding Style Guide](https://github.com/eventbrite/javascript/tree/master/react)
* [Airbnb React/JSX Style Guide](https://github.com/airbnb/javascript/tree/master/react)


#Redux and Mobx

**What's (Redux/Mobx)?**

* [Confused! Redux or MobX?](https://www.reddit.com/r/reactjs/comments/4npzq5/confused_redux_or_mobx)

**Do I need to use (Redux/Mobx)?**

* [You don’t need Redux if your data never changes. The whole point of it is managing changes.](https://twitter.com/dan_abramov/status/737036433215610880) Dan Abramov @dan_abramov
* [You Might Not Need Redux](https://medium.com/@dan_abramov/you-might-not-need-redux-be46360cf367#.kgnqdp8p6) Dan Abramov @dan_abramov
* [Redux or MobX: An attempt to dissolve the Confusion](http://www.robinwieruch.de/redux-mobx-confusion/) Robin Wieruch @rwieruch

**How to scale React-Redux apps?**

* [About folder structure, styling, data fetching, etc.](https://www.smashingmagazine.com/2016/09/how-to-scale-react-applications/) Max Stoiber @mxstbr
* [How to choose between Redux's store and React's state?](https://github.com/reactjs/redux/issues/1287)

#Adding React to an existing app

**How do I start adding React to an existing app?**

* [How to Sprinkle ReactJS into an Existing Web Application](https://scotch.io/tutorials/how-to-sprinkle-reactjs-into-an-existing-web-application) Andrew Del Prete @andrewdelprete
* [Don't Rewrite, React!](https://www.youtube.com/watch?v=BF58ZJ1ZQxY) Ryan Florence
* [Migrating Safely to React](https://www.youtube.com/watch?v=sXDZBxbRRag&list=PLNBNS7NRGKMG3uLrm5fgY02hJ87Wzb4IU&index=1) Jamis Charles



