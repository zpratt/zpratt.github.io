Building [React](http://facebook.github.io/react/) components for use with [google maps](https://developers.google.com/maps/documentation/javascript/reference) can present an interesting problem for those who aren't aware of the basics/quirks of developing with google maps. I aim to shed some light on the fundamentals of how to get the two to play nicely together, and to promote developing the components in a way that will promote testability as well.

## Why?

Out of the box google maps components are fine for simple use cases, such as, displaying a marker for a given Lat/Lng point and InfoWindows for descriptive content about a given point. However, things get interesting when the time comes where you need to be able to have full control over the style of a component, or to easily update content based on changes from the server. There are thirdparty libraries out there that will wrap the google map component primitives, but those have their own problems and often contain a bunch of bloat trying to handle all possible user interactions and browser quirks.

## Prerequisites

1. A basic understanding of spatial data primitives: coordinate systems, projections, basic geometric data types
2. A basic understanding of React
3. A basic understanding of google maps
4. A basic understanding of Grunt
5. A google maps API key

## Where we're going

As an introductory step, we will start by building a custom [OverlayView](https://developers.google.com/maps/documentation/javascript/reference#OverlayView) that is positioned by a point (as opposed to being positioned by a bounds, which is also possible). We will keep this simple by focusing on a basics using React with google maps and avoid fetching data from the server or binding UI interactions to a client-side router.

## Separating concerns

My preferred method for separating concerns when building custom OverlayViews is to start with the following pattern:

* Build a constructor function which inherits from the `google.maps.OverlayView` constructor.
* Implement the React component in such a way that it knows nothing about any of the google maps APIs
* Implement a facade, (in the spirit of the [Command Pattern](http://en.wikipedia.org/wiki/Command_pattern)) which abstracts away the complexity of the coordination that needs to occur between the OverlayView and the React component

## Digging in

### Implementing the OverlayView

### Implementing the React component

### Implementing the facade

## Using it

## Where to after this?
