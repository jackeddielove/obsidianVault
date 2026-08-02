# remember:

From the Pattern:
Today, reconnect with what first sparked your excitement about a goal or idea you've been sitting on. Your sense of adventure didn't disappear—it's simply waiting for you to call on it. Take aim, and let your optimism lead the way.

From somewhere, I don't know:
- Start with an empowerment promise, not a joke.
- Circle key ideas 3 times; people always miss things.
- Near-miss technique—show what almost looks right but isn't.
- 5S rule: symbol, slogan, surprise, salient, story. Hit at least 3.
- Fewer slides. Bigger font. No laser pointer. No reading aloud.
- End with contributions, not a summary or thank you.
- Passion is contagious. Talk about what genuinely excites you.
- Fence your idea. Show what it's not so it doesn't blur with others.

# Title
- [x] workbook
- [x] slides
- [x] materials (none)
# 0.0. Warm-up
- [x] workbook
- [x] slides
- [x] materials (none)
# 1.0. Infinity as a number
- [x] workbook
- [x] slides
- [x] materials
# 1.1. Comparing finite sets
- [x] workbook
- [x] slides
- [x] materials
# 1.2. Comparing infinite sets
- [x] workbook
- [x] slides
- [x] materials
# 1.3. Beyond infinity
- [x] workbook
- [x] slides
- [x] materials



# Warm-up (15 minutes)

- Ask for a volunteer. Count how many hi-fives happen when we hi-five each other. Start the whiteboard table.
- In your notebook, start the following table

| group size | high fives |
| :--------: | :--------: |
|    $2$     |    $1$     |
|            |            |
|            |            |
|            |            |
|            |            |
|            |            |
|            |            |

- Make two groups of 3 and one group 4. Ask the groups to count how many hi-fives occur in their groups. Continue table

| group size | high fives |
| :--------: | :--------: |
|    $2$     |    $1$     |
|    $3$     |    $3$     |
|    $4$     |    $6$     |
|            |            |
|            |            |
|            |            |
- Make two groups of 5 and ask them the same. Continue the table.

| group size | high fives |
| :--------: | :--------: |
|    $2$     |    $1$     |
|    $3$     |    $3$     |
|    $4$     |    $6$     |
|    $5$     |    $10$    |
|            |            |
|            |            |
- Question: How many hi-fives if all 10 of you hi-five each other? Take a few minutes to talk about it in your groups of 5.
- Discuss solutions while introducing function notations.
	## Solutions
	$$ H(n)=H(n-1)+(n-1)\qquad H(n)=1+2+3+\cdots+(n-1)\qquad H(n)=\frac{n(n-1)}{2} $$
	## Notations
	$$
	\begin{align*}
	H:\mathbb{N}&\to\mathbb{N} \\
	2&\mapsto 1 \\
	3&\mapsto 3 \\
	4&\mapsto 6 \\
	5&\mapsto 10 \\
	n&\mapsto H(n) \\
	\end{align*}
	$$
	An example of the ubiquity of this notation: pick a random paper from the [Arxiv](https://arxiv.org/list/math.AC/new), or a [specific one](https://arxiv.org/html/2605.21703v1):$$\begin{align*}
	\mu:\{\text{weighted homogenous polynomials of type }(w_1, \ldots, w_r; d)\}&\to \mathbb{Z}_{\geq 0}\cup\infty \\
	f &\mapsto \prod_{i=1}^r \frac{d-w_i}{w_i}
	\end{align*}$$

- Plug in $10$ to our formulas, and then check with an experiment.

# Intro (5 minutes)

Slide: Infinity as a Number

Q: What is a number? What is infinity?

Our answer (on a slide): A number is the answer to a "how many" question.
- How many people in this room?
- How many seconds in 24 hours?
- How many ants on the earth?
- How many atoms in the observable universe?
- How many counting numbers are there? $\{1, 2, 3, 4, 5, 6, \ldots \}$
- How many even counting numbers are there? $\{2, 4, 6, 8, 10, 12, \ldots \}$

This is what we're going to look at today: If infinity is a number, how does it work? What is $\infty+1$, $\infty+\infty$, $\infty\cdot\infty$, $\infty^\infty$?

In order to understand infinite sets, we first need to understand finite sets.

# Comparing finite sets

You each have an envelope with paperclips and rubber bands. Which are there more of? How do you know? Yes, you can count. But, we are soon going to work with infinite sets, where counting no longer is an option. How can you tell there are the same number of paperclips and rubber bands without counting?
We match them up! Go ahead and match them in front of you. Here's my matching (document camera).
You just created a **one-to-one correspondence**, also called a **bijection**.

Write this in your notebook:
*Two sets have the same cardinality if there is a bijection between them.*

Write this in your notebook:
$$\text{paperclips}=\{P_b, P_g, P_y, P_p\}$$
$$\text{rubber bands}=\{R_b, R_g, R_y, R_p\}$$
Claim: The sets "paperclips" and "rubber bands" have the same cardinality.
Proof: Here is a bijection between the sets.
$$\begin{align*}
f:\text{paperclips}&\to\text{rubber bands} \\
P_b &\mapsto R_b \\
P_g &\mapsto R_g \\
P_y &\mapsto R_y \\
P_p &\mapsto R_p \\
\end{align*}$$
Let's capture this information a couple more ways. Here's one:
 $$f(P_b)=R_b \qquad f(P_g)=R_g \qquad f(P_y)=R_y \qquad f(P_p)=R_p$$and here's another:

| $\text{paperclips}$ | $\text{rubber bands}$ |
|:-------------------:|:---------------------:|
|        $P_b$        |         $R_b$         |
|        $P_g$        |         $R_g$         |
|        $P_y$        |         $R_y$         |
|        $P_p$        |         $R_p$         |
*Can we take a moment to appreciate that we are doing math? There are no numbers, no formulas. It is really nothing more than an organization of information. In a sense, the entire project of mathematics is one of organizing information and discovering hidden pattern and structure.*

	What you've just done is you made a **one-to-one correspondence** between your set of beads and your set of stones. When there is a one-to-one correspondence between two sets, we say they have the same **cardinality**.
	We have notation for the cardinality of a set: $\vert A \vert$ is the cardinality of a the set $A$.
	So we can write $|\{\text{beads}\}|=5$, $|\{\text{stones}\}|=5$, and what we care about is
	$$|\{\text{beads}\}|=|\{\text{stones}\}|.$$
	
	Definition: Let $A$, $B$ be sets. A **one-to-one correspondence** between $A$ and $B$ is a map $f:A\to B$ such that every element of $B$ gets mapped to by exactly one element of $A$.
	
	Definition: Two sets $A$, $B$, have the **same cardinality** if there is a one-to-one correspondence between $A$ and $B$.
	
	Let's next compare these two sets:
	$$\{1, 2, 3, 4, 5\}\qquad\{2, 4, 6, 8, 10\}$$
	Do they have the same cardinality? What is an example of a one-to-one correspondence?
	$$\begin{align*}
	f:\{1, 2, 3, 4, 5\}&\to\{2,4, 6, 8, 10\} \\
	1&\mapsto 2 \\
	2&\mapsto 4 \\
	3&\mapsto 6 \\
	4&\mapsto 8 \\
	5&\mapsto 10 \\
	\end{align*}$$
	We can also write $f(1)=2, f(2)=4, f(3)=6, f(4)=8, f(5)=10$. In fact, we could say all of that with a single statement: $f(n)=2n$. Since we have a one-to-one correspondence, their cardinalities are the same:
	$$|\{1, 2, 3, 4, 5\}|=|\{2, 4, 6, 8, 10\}|$$
	
Now, work with your neighbor to prove that the sets $\{1, 2, 3, 4, 5\}$ and $\{2, 4, 6, 8, 10\}$
have the same cardinality. Anyone want to come up to the board and write down the bijection you came up with?

We're finally ready for our first definition of infinity: Infinity is the cardinality of the set of counting numbers. Write this down.
The set of counting numbers is denoted $\mathbb{N}$:
$$\mathbb{N}=\{1, 2, 3, 4, 5, \ldots\}$$
The cardinality of this set is a number we are going to call $\aleph_0$:
$$|\mathbb{N}|=\aleph_0$$

# Hilbert's hotel

(Note: maybe make the explicit bijections optional... at least, don't have a lot riding on them)

3D slide that shows "infinitely" many rooms (vacancy sign on). There's a room for every counting number. How many rooms are there? $\aleph_0$.
$$\text{Rooms}=\{R_1, R_2, R_3, R_4, R_5, \ldots\}.$$
Here is your own Infinite Hotel on paper (you have to use your imagination).

Infinitely many guests show up. They appear on the slide. There's a guest for every counting number. How many guests are there? $\aleph_0$.
$$\text{Guests}=\{G_1, G_2, G_3, G_4, G_5, \ldots\}.$$
Can all the guests check in? Is there a one-to-one correspondence between $\text{Guests}$ and $\text{Rooms}$?

Here are your guests (hand out bags of tiles). Go ahead and assign the guests to the rooms in the most natural way you can.

The guests move into the rooms on the slide. The bijection is revealed.
$$G_n\mapsto R_n$$

But the vacancy sign is still on. What's up with that?

So a new person walks up, $H_1$. Can $H_1$ have a room? Now we have
$$\text{Guests}=\{H_1, G_1, G_2, G_3, G_4, \ldots\}$$
$$\text{Rooms}=\{R_1, R_2, R_3, R_4, R_5, \ldots\}$$
Is there still a one-to-one correspondence between $\text{Guests}$ and $\text{Rooms}$? The front desk needs to know which key to give to each guest.
$$H_1\mapsto R_1, \, G_n\mapsto R_{n+1}$$
Ok, so adding $1$ to a set of cardinality $\aleph_0$ does not change its cardinality:
$$\aleph_0+1=\aleph_0.$$
What if $10$ new people show up?
$$\text{Guests}=\{H_1, H_2, H_3, \ldots, H_{10}, G_1, G_2, G_3, G_4, \ldots\}$$
$$\text{Rooms}=\{R_1, R_2, R_3, R_4, R_5, \ldots\}$$
Is there still a one-to-one correspondence between $\text{Guests}$ and $\text{Rooms}$?
$$H_n\mapsto R_n, \, G_n\mapsto R_{n+10}$$
$$\aleph_0+10=\aleph_0$$
## Drawing one-to-one correspondences

When you start doing $\mathbb{N}^2$ and $\mathbb{N}^3$ , make the tiles different colors so you get a pattern in your hotel