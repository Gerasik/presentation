## 1 slide 
React is a JavaScript library for building fast and interactive user interfaces.

## 2 Slide
It was developed at Facebook in 2011.

## 3 Slide
And currently it's the most popular javascript library for building user interfaces. 
As you can see on google trends react is dominating the space of libraries and 
frameworks for building user interfaces. The other two players here are angular and vuew.

## 4 Slide
### 4-1
At the heart of all react applications are components. 
A component is essentially a piece of the user interface.
So when building applications with react. 
We build a some of isolated and reusable components.
### 4-2
And then compose them to build complex user interfaces. 

## 5 Slide
### 5-1
Every react application has at least one component which we refer to as the root component.
This component represents the internal application and contains other child components.
So every react application is essentially a tree of
components.
If you have worked with angular 2 or higher it should sound familiar.

### 5-2
Here is an example.
Let's imagine we want to build an application like Twitter.
We can split this page into components like navbar, profile, trends and feed.
### 5-3
User a representation of these components in a tree.
So we have app and below that we have navbar, profile, trends and feed.
Now feed includes several tweet components, each tweet component can include a 
like component which we can reuse on other pages or even in different applications.
So as you see each component is a piece of UI. We can build these components 
in isolation and then put them together to build complex UIs.

## 6 Slide
### 6-1
In terms of implementation a component is typically implemented as 
a JavaScript class. 
That has some state and render method. 
The state here is the data that we want to display when the component 
is rendered and the render method as you can tell is responsible for describing what the UI should look like.
### 6-2 
The output of this render method is a react element which is a 
simple plain JavaScript object that maps to a Dom element. 
It's not a real Dom element, it's just a plain JavaScript object that represents that Dom element in memory. 
So react keeps a lightweight representation of the Dom in memory, which were referred to as the virtual Dom. 
Unlike the browser or the real Dom this virtual DOM is cheap to create.
When we change the state of a component we get a new react element. 
React will then compare this element and his children with the previous one it figures out what is changed 
and then it will update a part of the real Dom to keep it in sync with the virtual Dom. 
So that means when building applications we react unlike vanilla JavaScript or jQuery we no longer have to 
work with the Dom API in browsers.
In other words we no longer have to write code in query and manipulate the Dom or attached event handlers 
to Dom elements. 

## 7 Slide
It's simply change the state of our components and react will automatically update the Dom to match that 
state. 
And that's exactly why this library is called react. Because when the state changes React essentially 
reacts to the state change and updates the dumb. 

## 8 Slide
One of the popular questions is the React or Angular.
Well both react and angular are similar in terms of their component based architecture. 
However angular is a framework or a complete solution while react is a library. 
It only takes care of rendering the view and making sure that the view is in sync with the state. 
Let's all react does nothing less nothing more.
For this very reason react has a very small API to learn. 
So when building applications with react we need to use other libraries for things like routing or 
calling HTTP services and so on.
But this is not necessarily a bad thing because you get to choose the libraries that you prefer as 
opposed to being fixed with what angular gives you which often breaks from one version to another. 





