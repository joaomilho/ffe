## Functional front end

It's common knowledge that front end development sucks. Can we fix it? No. But can it at least be functional? Yes.

This is a presentation will go over the recent history of front end development, and why now so many attention has been given to functional programming.

My main argument will be this:

1. The possibility of declarative DOM trees (a.k.a. virtual DOM) allows the UI to be a pure function of a given state. This pattern is the foundation for a functional programming style.
2. Given the web is an event-driven, asynchronous environment, this style of programming is highly desirable.

The plot will be this:

1. I'll go over the basics of [Elm](http://elm-lang.org), a programming language inspired by [Haskell](https://www.haskell.org) with a strong focus on functional reactive programming for the web. 
2. I'll try to explain the signal system behind Elm, but will focus more on the Elm architecture (a.k.a MVU, or model, view, update). The goal is to convince you that reasoning with this architecture is much simpler than the common alternatives, since a) all updates are pure functions b) the view is a pure result of the application of a given model state, c) the model is very explicit and d) every event that causes updates are also very explicit and not spread all over.
3. I'll show a little bit of Elm's tools to visualize your app;
4. I'll turn to more mainstream technology, [React](http://facebook.github.io/react/) and demonstrate how [almost] the same things can be accomplished using it along [Redux](https://github.com/gaearon/redux).

The main goal is:

1. To convince Javascript developers that learning some [Haskell](https://www.haskell.org) (well, Elm, which is very similar) gives you a pure, infinite and immutable source of insights. 
2. To show that functional front end is here to stay.

### Content

###### Slides

The source slides can be downloaded [here](https://github.com/joaomilho/ffe/blob/master/functional-front-end--the-konference.key?raw=true), but you'll need [Apple's Keynote](https://www.apple.com/mac/keynote/). A [PDF is also available](https://github.com/joaomilho/ffe/blob/master/functional-front-end--the-konference.ffe), but it probably looks bad.

###### Code

The code is, well... in this repo. The best way to visualise it is using the awesome [Git Wayback Machine](https://github.com/MadRabbit/git-wayback-machine).

Also I may show you a little bit of these projects:

  - [github.com/joaomilho/game-of-life-elm](https://github.com/joaomilho/game-of-life-elm)

  - [github.com/joaomilho/kevernote-elm](https://github.com/joaomilho/kevernote-elm)

  - [github.com/joaomilho/kevernote-elm](https://github.com/joaomilho/kevernote-redux)
  
### Resources

###### Elm resources

  - [Online Elm REPL](http://elm-lang.org/try)

  - [Elm's StartApp docs](http://package.elm-lang.org/packages/evancz/start-app/1.0.1)

  - [The Pragmatic Studio's Elm Course](https://pragmaticstudio.com/elm)

  - [Elm's Subreddit](https://www.reddit.com/r/elm/)

###### Elm tutorials

  - [Checkerboard Grid Tutorial](https://github.com/TheSeamau5/elm-checkerboardgrid-tutorial)

  - [Elm's architecture](http://elm-lang.org/guide/architecture)
  
###### Presentations

  - [Shipping a Production Web App in Elm](https://presentate.com/rtfeldman/talks/shipping-a-production-web-app-in-elm) *by* [Richard Feldman](https://twitter.com/rtfeldman) WARNING: Cat overflow
  
###### Videos (sorted as a suggestion)

  - [Simplicity Matters](https://www.youtube.com/watch?v=rI8tNMsozo0) *by* [Rich Hickey](https://twitter.com/richhickey)

  - [Reactive Extensions for JavaScript](https://channel9.msdn.com/Events/MIX/MIX10/FTL01) *by* [Eric Maijer](https://twitter.com/headinthebox)
 
  - [Live React: Hot Reloading with Time Travel](https://www.youtube.com/watch?v=xsSnOQynTHs) *by* [Dan Abramov](https://twitter.com/dan_abramov)

  - [Controlling Time and Space: understanding the many formulations of FRP](https://www.youtube.com/watch?v=Agu6jipKfYw) *by* [Evan Czaplicki](https://twitter.com/czaplic)  

  - [My adventure with Elm](https://www.youtube.com/watch?v=cBVXyxt-9_Q) *by* [Yan Cui](https://twitter.com/theburningmonk)
  
  - [PureScript (Maybe This Time We Get JavaScript Right)](https://www.youtube.com/watch?v=yIlDBPiMb0o) *by* [Bodil Stokke](https://twitter.com/bodil)
  
  - [Let's be mainstream! User focused design in Elm](https://www.youtube.com/watch?v=oYk8CKH7OhE&feature=youtu.be) *by* [Evan Czaplicki](https://twitter.com/czaplic)
  
  - [The Essence of FRP](http://begriffs.com/posts/2015-07-22-essence-of-frp.html) *by* [Conal Elliott](http://conal.net/blog/)

  - [Functional Frontend Frontier](https://www.youtube.com/watch?v=06M0jdYYSis) *by* [Richard Feldman](https://twitter.com/rtfeldman)

  - [What does it mean to be Reactive?](https://www.youtube.com/watch?v=sTSQlYX5DU0) *by* [Eric Maijer](https://twitter.com/headinthebox)

  - [Duality and the End of Reactive](https://channel9.msdn.com/Events/Lang-NEXT/Lang-NEXT-2014/Keynote-Duality) *by* [Eric Maijer](https://twitter.com/headinthebox)

  - [Fundamentalist Functional Programming](https://www.youtube.com/watch?v=UuamC0T3hv8) *by* [Eric Maijer](https://twitter.com/headinthebox)
