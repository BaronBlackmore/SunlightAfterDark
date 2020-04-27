---
layout: post
---
Unity has some fairly cumbersome back-and-forths between different places in the program where you have to specify different things, a lot of important things are hidden, but that's mostly because there are just so many tools available.
There are plenty of good resources if you'd like to learn to use these tools or make a game in a following the steps kind of way. The problem came when I would try to make something of my own, I was absolutely paralyzed, unable to know where to start.

Until something clicked, and in an instant I understood what was going on

It's all about boxes and addresses.

In this order of a few steps, If you want to make a thing, you have to:

1. Decide what shape of box it will fit in.
2. Give your box a name.
3. Fill the box with that kind of thing.
4. Use or its edit the contents.

And the steps must be done in this order for something to exist and work.

[boxes](/images/code-boxes.png)

Let me break this down. When you see something like:

````C#
public int myFavoriteNumber;
````

What this is saying is that we have an "int"(code word for "integer") box called "myFavoriteNumber" which we can change from anywhere (public). (btw, the strange way of writing this is called [Camel case](https://en.wikipedia.org/wiki/Camel_case) and Unity will turn "myFavoriteNumber" into "My Favorite Number" by itself when you view it from outside of the code editor).

Then step three is to fill the box with something that will fit into it. you could do this in the script or let that be done in the unity editor:

````C#
myFavoriteNumber = 5;
````

[Unity inspector screenshot](/images/sea-sharp.png)

Then step 4, since now that you have a box full of things and it has a name, you can ask for this box and it's contents from other places.
What's useful is that name isn't just a name but an address. myFavoriteNumber lives in the script it's written in, which is usually called a *class*, but you can think of it like a bigger box. You can tell which box is inside which because the bigger box wraps brackets around the small one (notice the curly brackets).

````C#
public class ReallyCoolMath{
	public int myFavoriteNumber;
}
````

In unity addresses are simple, they're just like post, except in reverse and with a period instead of a new line. To access myFavoriteNumber from somewhere else, you'd get it like this.

````C#
//first setup a box for it to go into
public int aCoolNumber;

//then fill it
aCoolNumber = ReallyCoolMath.myFavoriteNumber;

//or do both at the same time
public int anotherCoolNumber = ReallyCoolMath.myFavoriteNumber;
````

It's like if I want to give you a cup of tea, I first need to define what a cup is, call it something, and than fill it with tea. The tea is at my house, of course. And let's say i've left the door unlocked for you (public). So to come get it you'd write something like this:

````C#
public class MyHouse{
	public cupoftea teaForYou = earlgrey;
}
````

Only then can you I give you the tea. 