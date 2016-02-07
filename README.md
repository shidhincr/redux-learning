Redux
-------

When Facebook announced ReactJS in 2013, they also introduced a new architectural pattern called as Flux. Facebook gave the the idea of Flux to the world for efficiently handling the data a web application. However, it was just a pattern and Facebook allowed others to come up with libraries/framework implementing Flux. A number of Flux libraries evolved from then and some of them became very popular. [Redux](http://redux.js.org/) is an opinioated Flux variation and the tagline is "**A predictable state container for JavaScript apps.**"

Why this Guide
---------------

Unlike some of the new libraries, Redux has a wonderful documentation. Its author [Dan abramov](https://twitter.com/dan_abramov) has also published a free 30 videos course in Egghead.io. There're a number of articles about learning Redux. Here're some of the popular to get started:

1. [Redux documentation](http://redux.js.org/)
2. [Egghead.io course](https://egghead.io/series/getting-started-with-redux)
3. [Redux step by step tutorial](https://github.com/happypoulp/redux-tutorial)
4. [Full stack redux tutorial](http://teropa.info/blog/2015/09/10/full-stack-redux-tutorial.html)

Although there're all these wonderful articles out there, I felt a beginner's guide is missing. You should be able to start with any new redux boiler plate project, but in most of them you might find code for configuring store, using middlewares, mapping state to props, binding action creators ..etc.

Here, my attempt is to understand what exactly each of these are trying to solve. To do that, we need to start from a basic app with out Redux, then introduce each Redux concepts step by step. This guide is all about that.

Contents
---------

The idea is to make a simple `Counter` component in React. It is divided into these sections:

- **Section 1** : React with state ( not using Redux ).
- **Section 2** : Try to integrate Redux and using store.
- **Section 3** : Using React-redux library to connect between React and Redux.
- **Section 4** : Removing boilerplate code with redux helper methods.
- **Section 5** : Async code handling with middlewares.

Contributing
-------------
To be honest, I am not a good writer. If you feel something is not right, please open a PR. I'll gladly accept and appreciate any kind of contributions -- from a typo to complete re-write of any sections in this. If you've any questions, open it as a new issue.

Thanks
-------
To the great React and Redux community.
