
talking points for ted meeting
	background
		i grew up wanting to be an artist or maybe an architect, some creative field. then i found skateboarding and just wanted to do that, and i didn't go back to school til i was 25 or so. my math classes were a lot of fun and i loved the visual aspects of calculus so i decided to major in math. berkeley was a bit of a whirlwind but i did enjoy the increasing generalization of the ideas i had learned about in lower-division courses, and mathematics as phenomenon became more and more interesting. i decided to get a masters with the intention of teaching at a community college. during my masters i did some original research and also developed activities for k12 students that introduced so-called advanced mathematical ideas in fun and interactive ways. from there i went on to a phd program and continued doing this work of communicating mathematics to non-mathematical audiences. since then i'v gone back to get a design degree, have taught at ccsf and sfsu, and continue to make mathematical art.
	interests
		i have these three things that i love doing: making, learning, and teaching. And most of my projects involve all three. i may eventually have a physical space where i can make work and host workshops and classes, but for now i'm doing this sort of low overhead, in the streets style, just going into classrooms and sharing the stuff that i find fascinating with others.
	Intro
		it's called making space: the mathematics of higher dimensions
		the goal here is to both introduce and demystify the notion of higher dimensions, because from a mathematical point of view they are every bit as ordinary as the 2- and 3-dimensional spaces we're familiar with
	part 1
		in the first part we look at things we're familiar with in 2- and 3-dimensions and we look at how we describe those these with numbers. we spend a lot of time here to really get comfortable with this idea, and part 1 ends by extending these ideas to higher dimensions in a really simple way
	part 2
		then in the next part we try to get an idea of what these 4-dimensional things look like. it's one thing to just invent them as natural extensions of 3-dimensional things, but do they exist in the way that 2- and 3-dimensional things exist
	part 3
		in the last part we see how mathematical space is much broader an idea than physical space. physical space is just one manifestation of mathematical space. for example, a point in 3-dimensional mathematical space may correspond to a point in 3-dimensional physical space, but it can also represent a color. or a point in 4d mathematical space can represent a rotation physical 3d space--this idea is used in computer graphics. or you could do something like, say you have 5 different activities you're gonna do today: do homework, play basketball, write some poetry, watch netflix, and help out around the house. and say you're gonna spend between 0 and 60 minutes on each one. you just defined a 5-dimensional cube, and every point in that cube is a potential way to spend your day. There's a whole field called linear programming where you have a bunch of variables like this and the space of possible solutions is some kind of high dimensional geometric object. Often times you want to maximize or minimize some particular variable or combination of variables, and this amounts to running a high dimensional plane across your high dimensional geometric object until you reach a certain point that optimizes your solution.
	
to do
	make sure mouse/controller has full batteries
	do a trial run with some folks
	make rotate buttons turn each other off
	something buggy with the 3d slices of the 4d cube around w=0
	final slide
	highlight rotations planes and change rotate x, rotate y, rotate z to rotate yz, rotate xz, rotate xy
	names for Tuesday: Jenifer Fried
	**Tuesday 4/15:**
	- 9:45- 10:15- Burnett math 8 P6 room 205
	- 10:15-10:45- Math 8 room P6 305
	- 11-11:30- Burnett math 8 P7 room 205
	- 11:30-12- Sandoval math 6 P7 room 5
	**Thursday 4/17**
	- 1:30-2:00 Burnett P2 8th grade math room 205
	- 2:00-2:30 Sandoval P2 6th grade math/sci room 5
	- 2:00-2:30 Thomas Lopez P2 7th grade math room 305
	- 2:45-3:15 Thomas Lopez P3 7th grade math room 305
	- 3:15-3:45 Mr. Sandoval P3 6th grade math room 5
	**Friday 4/18**
	- ~~10:15-10:45 P4 Burnett 8th grade math room 205~~
	- 10:45-11:15 P4 Sandoval 6th grade math room 5
	- ~~11:30-12:00 P5 Burnett 8th grade math room 205~~
	- 12:00-12:30 Thomas Lopez 7th grade math room 304
show sub-cubes
make things playful--leave possibility open
talking points
	Intro
		What does the word dimension mean? What is 2d, and 3d? is there a 4d, 5d, 6d?
	Part 1
		in this first part we're going to look at how mathematicians use numbers to talk about space. actually we use them to *create* space.
		**2D**
		here are some simple objects you know about in 2D space. (turn on each one) let's see how we make each one with numbers.
		POINT
		can anyone tell me the coordinates of this point? great, (5, 3). this is a huge conceptual leap. we just took an object in space and turned it into a pair of numbers. now, which one is the actual point? is it the blue dot, or is it the pair of numbers? mathematics is this interesting way of interacting with the world, where it's a back and forth between the "real world" of our experience and a mathematical world that we create.
		ok so a point is pair of numbers, here's a table where we'll keep track of objects and their mathematical representations. now back to our 2d space
		LINE
		here's a line. now this line is just a bunch of points, is it not? let's drag our blue point along the line and highlight some of them. ok so the line is a bunch of points, and each point is a pair of numbers, so the line is just a bunch of pairs of numbers. which pairs are they? the answer is given by this equation. now which thing is the line? the green drawing on the screen, or the equation? the way we go back and forth, this metaphor, is becoming more productive. a point is a number pair and a line is a linear condition. but moreover, a point is on a line if the number pair fits the linear condition.
		here's the next row in our table
		SQUARE
		ok, one more object, a square. what are the points at the corners? what are all the points inside? describing all the points in the square with numbers is a little bit more involved than describing all the points on a line, so let's just keep track of the corners for now. that will be enough. notice that each corner is a combination of 0s and 1s. we could also notice that the edges are either x=0, x=1, y=0, or y=1. 
		here's the square interpreted in the world of numbers
		one last thing to mention: we can rotate this square, right? but if the square is just a bunch of pairs of numbers, how do we know how those numbers change when we rotate it? we don't have time to go into it, but there is something called a rotation matrix, and all we need to know is that it doesn't actually rotate the square, it just operates on the numbers. but when we let it operate and then we look at the new numbers, we get a rotated square.
		here's how we use numbers to rotate
		**3D**
		let's look at the 3d versions of the objects we just explored in 2d.
		POINT
		if a point in 2D is a pair of numbers, what is a point in 3D? yup, just 3 numbers. let's call them x, y, and z. here's the start of our 3D table
		PLANE
		remember what a line was in 2D? ax+by=c, right? we called it a linear condition. what do you think a linear condition in 3D is? yup, you got it, just throw a z in there with its own coefficient. here's what it looks like. let's play that same game where we try to find points on the plane, in other words, triples that fit the linear condition. let's start with 1x+1y+1z=3. ok so a point is on a plane if the triple satisfies the linear condition
		CUBE
		a cube is just a 3d version of a square. what are the vertices? what about the faces? what about the edges? We can also rotate the cube but now there are more options. We can rotate it this way, or this way, or this way, and every orientation of the cube is some combination of these three basic rotations.
		**TABLE**
		Here's where we are so far. we have points, planes, and cubes in 2D and 3D (a 'plane' in 2D is called a line, and a 'cube' in 2D is called a square). there are patterns here, right? can't we extend these patterns and call the new objects 4D points, planes, and cubes? This is another interesting feature of mathematics: the ability to generalize. Once we take things that we know from our experience and describe them mathematically, we can often generalize those descriptions to create new objects we've never seen before. An interesting question is "what *are* those new objects", or, "what are they good for?" In the next section, we will try to understand more about what this 4D cube "looks like".
		use orbit control to star wars that shit
	Part 2
		**PROJECTING 3D TO 2D**
		Here's another picture of that 3D cube from before. Imagine you are a 2D person living in the 2D world down here. Here's another picture of your world up here in the corner. you can't see the cube above you--in fact, "above" doesn't even exist in your vocabulary. But you just had a math demonstration in your 2d classroom where someone told you there is a third dimension and you can use three numbers x, y, z to describe this space and there's a 3D version of a square that's called a cube and you can describe its vertices with numbers and you can rotate the cube, again using numbers. and you can see its shadow (you guessed it, casting a shadow is also done with numbers)
		**PROJECTING 4D TO 3D**
		Ok, now we're back in our 3d world but a 4d person is telling us there's a fourth dimension, you can describe it using 4 numbers x,y,z,w, and there's a 4d version of a cube and you can describe it's vertices with numbers and you can even rotate them using 4d rotation matrices. notice how if i just rotate in the xyz world, the shadow just rotates but it doesn't change shape. this happened with the 3d version too, right? and what happened in the 3d version when we rotated out of the 2d plane, we got these sorta squares passing through each other. so what's gonna happen when we do that here? we get these cubes passing through each other. then finally, we did combined rotations and we got to see a more full picture of the 3d cube projected onto our 2d world. so let's see what this thing actually looks like.
		**SLICING 3D WITH 2D**
		ok, here is another way to peer into higher dimensions. instead of taking shadows, we can take slices. keep in mind that we are 2d people so we can't see this 3d cube, it only exists for us mathematically, that is, in terms of numbers. i can move it up and down with numbers (even though up and down are new concepts to us). and as it passes through our 2d world, i can use numbers to draw the part of it that we can see.
		notice how it changes shape. it starts as a triangle because three of the edges are passing through. each edge intersects with our world as a single point, and when we fill in the resulting shape we get a triangle. then when we get to the ends of those edges, each one splits into two new ones so we get 6 edges now passing through. again each edge passes through our world as a single point, so we have 6 points and the resulting shapes are different kinds of hexagons. then each pair of edges collide into a single edge and we're back to triangles until it finally disappears out of view.
		**SLICING 4D WITH 3D**
		well you see where this is going. instead of first seeing a 3-pointed 2d figure, we're going to see a 4-pointed 3d figure. then the first change happens when the four edges trifurcate so we get a 12 pointed figures. then there's an instant when those 12 collide in pairs giving a single 6-pointed object before immediately doing the complementary thing (back to 12, then 4, then disappearing) on the way down.
	the (x,y) is the point. the picture of the point is one of many possible representations of the mathematical point. the xy-plane is one of many possible representations of mathematical 2d space
	this point is on this line <--> this pair of numbers fits this linear condition
	how different generalizations give different branches of mathematics, with different applications
	see how rotate x, rotate y, just gives squares/rectangles, and rotate z doesn't change the shape?


rgb slide: if rgb is off and curveX is on, can't turn off curveX
right arrow keeps going after last slide
put a period at the end of the presentation (metaphorically):
	the fourth dimension exists (we create it with our imagination and numbers)
	there are 4D versions of familiar 2D and 3D objects
	we can peer into the 4th dimension by looking at shadows and slices
types of interactions:
2
	clicking buttons (ternary)
	dragging point
	changing coordinates
	selecting lattice points
3
	bullet points
4
	clicking buttons (binary and ternary)
5
	bullet points
6
	sliding table
8
	clicking buttons
	rotations
9
	clicking buttons
	rotations
10
	scroll translate
11
	scroll translate
13
	dragging sliders
	clicking buttons
	trace curve
slide0
	constructor
		titleTimer
		phi_x, phi_y, phi_z
		P=[p_0, ..., p_{15}]
		**cleaner names**
	functions
		titleRotation(a, b, c, v)
			uses arrays, can't have 4D vectors--but output can be vector
			**make output a vector**
		show()
			background
			text
			rotating 4-cube
slide1
	no constructor; just show text
slide2
	constructor
		gridpts array (**clean up indices**)
		sqColor color
		coefficients array
		buttons values
		ptCoords array
		**cleaner names**
	mouseClicked
		buttons
		lattice points (**clean up indices**)
	mouseWheel
		coefficients
	worldToScreen
		belongs in helper functions
	f(x)
	show()
		background
		buttons
		axes with tics
		grid (interactive)
		point
		line
		square