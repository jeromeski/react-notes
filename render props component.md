OK, guys, so in this lecture, we will talk about render props.

Why do you use it and how to use it?

So if we start by defining what is render props component, we can say that render props component

is that component that takes a child, render function.

So the child of this render promp component is a render function that tells this.

Render prop.

How to render.

OK.

So why are render props?

First of all, render props allows you to COMMUNICATE BETWEEN YOUR PARENT AND CHILD by passing the child.

Any arguments we want?

Second, by using render props, we can keep SEPARATION OF CONCERNS

So the parent can hold a special logic that the child does not have to know.

Another benefit from render props is a design pattern benefits.

So by using render props, we can SEPARATE LOGIC LAYER FROM VIEW LAYER.

Another good reason that we want to use render props is dependency injection.

The parent can INJECT THE CHILD ADDITIONAL INFO AND DATA TO VIEW also render props will allow

you to REUSE YOUR PARENT LOGIC ACROSS MULTIPLE VIEWS COMPONENTS so you can reuse your render props component

by using it in multiple view components.

So the best way to understand what is under prop component is just by looking.

Good example.

So let's see our example.

Let's look at this component.

OK, so this component is called deleteItem.

And if we look at the return, we have it div with onMouseEnter and onMouseLeave event handlers.

And inside this container, we have a title and a button.

And the title says that if you want to delete it, you should click on this button over here.

And when we are entering this container, we have mouseEnter Event Handler.
so this mouse event handler will set our state with visible through.

So when we enter with the mouse through this container, we will get this DIV over here with a warning.

And when we leave, we will hide the warning.

So this is a very simple component that will show you warning whenever your mouse will enter this container.

And this container includes a button that will delete some item, let's say we want to reuse this logic.

So we want to add this logic to multiple view components that have a delete button.

So first of all, what we want to do is we want to take the view and just create a new component.

So let's take the view and just create a new component called delete button.

And this delete button.

What on?

Will return.

The view component over here.

So let us delete the view component from the parent.

So what we did.

We extracted the view layer from the delete item component because we want to ABSTRACT the delete item

component.

So we want to make the delete item component a RENDER PROPS COMPONENT.

So as we said at the beginning of this video, render props component is a component that accepts render

function as a child.

So.

The props of that need item is the children and the children is render function.

So what do we want to do is we want to return.

This function.

Because the children is a function that will render for us some specific view.

So what we want to do is we want to pass to these children these functions and the warning state object.

So we can pass to the children.

The warning and we want the show warning.

And the hide warning.

So.

In this line, you can see that this is actually a DEPENDENCY INJECTION.

So we are injecting to our children these properties.

So our delete item, we can just also changed the name because we obstructed this component so we can.

Name these delete warning.

Because it actually shows a warning.

So the delete warning now is under props component because it takes children and then it will render

the children and inject the children some additional information.

OK.

So what do you want to do now is we want to use the delete warning, render props component.

So as I said before, we have the delete button and delete what on.

Also would like to show warning.

So in order to add to this delete button to show this warning.

We want to use the delete warning render props component in this view.

Layer component.

So.

Into return, we want to use the delete warning component.

Let's just close it.

And.

So here we used the delete warning.

And we are passing it to the delete warning.

A child over here.

But as we said, the child should be a function.

So here we are going to write a function.

So let's open curly brackets.

And we want to declare over here function.

And this function will return this div container.

Making it clear.

So inside our delete warning, we passed a child and this child is a function, is an error function.

And these are a function will return react elements.

But now we want that this child.

To get these values from the delete warning.

So.

If we can't see up, we can see that the children is being rendered and past these arguments over here.

So we can access these arguments inside our child.

So let's just copy these arguments and and add them here.

So what we did is in our delete button, we used our render props component that is called delete warning.

And the warning is a component that will accept a child.

And this child is a function.

So this is our function.

And this code over here, this is our function is our children inside our delete warning.

So the delete warning will accept all this and then in return, it will execute this function.

And that's some arguments.

So these arguments are the injected properties to the child.

So here is a child that is the delete button can access these properties.

And then we can render our view component.

So this is a very basic example of render props.

And.

If we just go back and check our key points that we so in the beginning of this lecture.

First of all, we can see that we can communicate between the delete warning and the delete button so

the delete button can have access to these properties that the delete button took from the warning from

its parent.

So now if we have multiple delete buttons in our application, we can create another delete button.

Or delete icon.

So this delete icon will have some icon over here.

And this icon, we just wrap it with the delete warning render props component.

So now we can reuse this logic across our application.

One thing we can do also if if our warning this live over here is a consistent component that we want

to show in all view layers in our application so we can so we can take this live over here and just

call it warning component.

And this warning component, it can be passed from there and their props component.

So here we can pass a warning component and we can define this one in component.

As a component that will return our d'Hiv.

And it can be warning.

So what we did is we can pass also the warning if you component from the parent so the child would not

need to implement this warning component that we want to show to the user.

And also, we can go to the delete icon and that's it to the delete icon.

So here we have the warning component.

So this is an example for and their props component.

And you can find this example in our project.

And if you just expand your examples, you can see they're in their props.

Fine over there.

OK, guys, so I recommend using Grinder props because it have many benefits that will make your project

or make your components reusable and consequently make your project more maintainable.