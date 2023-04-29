# Redux-vs-Mobx

Hello everyone!

In this repo, I am going to compare two libraries designated to React (i.e. [Redux](https://redux.js.org/introduction/getting-started) and [Mobx](https://mobx.js.org/getting-started))
Both library is related and specified to storing data in React along with other state management techniques. I suggest you to refer to [other repo](https://github.com/samanshahin/Single-Page-App-in-ReactJS) of mine to know how to use redux in detail. 
so, If you search on the internet for these two libraries and do some real project as I did, you reach a list of cons and pros as below:

## Redux

The structure of how the library is working is in the repository I just mentioned above is like this:

![redux store](https://user-images.githubusercontent.com/75519159/235317614-b48eabe4-228e-48ca-a942-eaaffacc2803.png)

The description is simple:
Suppose 'store' as a watermelon and 'slicers' as pieces of it containing 'reducers', and 'data', to be used in a 'component' as a plate.
Or imagine 'store' as a 'database', 'tables' as 'slices', 'queries' as 'reducers' and 'data', to be used in html view...
You can find other description of how things are working on the internet, like these:

![Google-Doc-GIF](https://user-images.githubusercontent.com/75519159/235317780-43b111b5-f76a-4c5b-8b38-d2bf0b02fb1e.gif)

or this in comparison to Flux:

![53610441-d48ca180-3c05-11e9-8f1f-21180a50d524](https://user-images.githubusercontent.com/75519159/235317786-463cf7a6-c419-4c53-a873-6839aeed0f3f.png)

But MobX is a little bit different:
as it's being mentioned in its official guide, it is supposed to be simpler and more scalable. I'm telling you that I agree with them in first term but scalability is a bit tricky and shoule be tested on huge applications. Frankly I didn't test it on large and compliceted databases but MobX official website claimed that it''s 100% sure that it's scalable. At the time of providing this repository, I've never seen companies use MobX as their state management in React world.

![Mobx store](https://user-images.githubusercontent.com/75519159/235317823-bc941251-7379-44e7-a934-427fcabb8f2f.png)

another graph is:

![sheme-1](https://user-images.githubusercontent.com/75519159/235317996-28476419-2309-47f5-90f0-3ad52cb7aa08.png)

finally you can find a good sample of MobX at [this repo](https://github.com/mweststrate/state-routing-blog-sources/tree/master/src).
## Now comparison
- Redux is more structural with all parts seperated but MobX is seeking for simplicity and user-friendly environment by putting everything on sight.
- the coding is easier to be learnt in MobX thatn Redux, but once you followed the structure above I presented and [my repo](https://github.com/samanshahin/Single-Page-App-in-ReactJS) you'll be sure that it's too easy to learn how Redux works.
- Redux has been proved to be scalable even when you have several databases and it seems complicated and tiring to integrate them. But MobX is not that way. It's been claimed that it supports full scalability but I don't think so! Sorry bros...
- The store is more conotrollable in Redux than in MobX
- in Redux you should wait for a component to be mounted (ComponentDidMount() function) but in MobX, it's been rendered before the component loads. Cool yeah but be careful of server CPU, memory usage and bandwidth consumption.


Have Fun!
