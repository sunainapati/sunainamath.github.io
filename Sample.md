/* 
    from https://github.com/SnowPanda1024/snowpanda1024.github.io/tree/main 
*/ 

---
layout: page
_title: Sample
permalink: /misc/sample
---
This page is meant to test the various constructs available to this blog.

# Math
## Math Redering
This blog uses MathJax for rendering math. 

### Inline Math
Inline math may be delimited by `$` or by `\\(` `\\)`. For example:
```md
This is math: $x^2 + y^2 = z^2$, and so is \\(x^2 + y^2 = z^2\\). Also, \$4 works.
```
This is math: $x^2 + y^2 = z^2$, and so is \\(x^2 + y^2 = z^2\\). Also, \$4 works.

### Display Math
Display math may be delimited by `$$` or by `\\[` `\\]`. For example:
```md
This is display math: $$x^2 + y^2 = \boxed{z^2},$$ 
and so is \\[x^2 + y^2 = \boxed{z^2}.\\] 
```
This is display math: $$x^2 + y^2 = \boxed{z^2},$$ and so is \\[x^2 + y^2 = \boxed{z^2}.\\] 

**Note**: `$$` doesn't seem to be working though it is supported by Mathjax. May be Kramdown is interfering. Need to investigate later.

**Note**: In the above two examples, we had to use double `\\` instead of single `\`.

### Align and Align*
```tex
\begin{align}
a^2 + b^2 &= (a + b)^2 - 2ab, \tag{1}\label{eq:1} \\\\\\\\
a^2 - b^2 &= (a + b)(a-b).
\end{align}
```
\begin{align}
a^2 + b^2 &= (a + b)^2 - 2ab, \tag{1}\label{eq:1} \\\\\\\\
a^2 - b^2 &= (a + b)(a-b).
\end{align}
```md
And the equation can be referenced as $\ref{eq:1}$.
```
And the equation can be referenced as $\ref{eq:1}$.

**Note**: `\\\\\\\\` is needed for newline instead of `\\`.

**Note**: Align isn't doing numbering by default.

### Colors
Colors inside math can be done using `\color` or `textcolor`; e.g.
```md
This is $\color{red}{Red}$, as is $\textcolor{red}{Red}$.
```
This is $\color{red}{Red}$, as is $\textcolor{red}{Red}$.

However, for colors outside of math, it is better to use HTML and CSS; e.g.
```md
This is <span style="color:blue">some *blue* text</span>.
```
This is <span style="color:blue">some *blue* text</span>.

## Text Environments for Math
For text environments for math, we use HTML and CSS. Essentialy, we use an HTML element such as `div` and specify it's `class` to be one of `theorem`, `lemma`, `claim`, `example`, `definition`, `proof`. We can also provide an optional attribute `text`.

E.g.
```md
<div class='theorem' text='Fermats Little Theorem'>
If $p$ is a prime number, then for any integer $a$, the number $a^p − a$ is 
an integer multiple of $p$. In the notation of modular arithmetic, 
this is expressed as
\[a^{p}\equiv a{\pmod {p}}.\]
</div>
```
<div class='theorem' text='Fermats Little Theorem'>
If $p$ is a prime number, then for any integer $a$, the number $a^p − a$ is an integer multiple of $p$. In the notation of modular arithmetic, this is expressed as
\[a^{p}\equiv a{\pmod {p}}.\]
</div>

**Note**: Inside a HTML element such as `div` above, we don't need `\\[` and `\[` works. Similarly, `\\` for newline in align works. This is because Kramdown is not processing the items inside div. This also implies that markdown constructs such as `**` won't work inside HTML elements.

<div class='lemma'>
Let the incircle of triangle $ABC$ touch side $BC$ at $D$, and let $DT$ be a diameter of the circle.
If line $AT$ meets $BC$ at $X$, then $BD = CX$.
</div>

<div class='claim'>
    Let $I$ be the incenter, $H$ be the orthocenter, and $O$ be the circumcenter. Then we have the following:
    <ul>
<li>$\angle BOC = 2 \angle A$.</li>
<li>$\angle BIC = 90 + \frac{\angle A}{2}$.</li>
<li>$\angle BHC = \angle B + \angle C$.</li>
</ul>
</div>

<div class='example'>
    Prove that $\frac{a+b}{2} \ge \sqrt{ab}$.
</div>

<div class='definition' text='Fixed Point'>
A configuration $x$ is a fixed point of an action $g$, if $g \cdot x = x$. The set of fixed points for $g$ is denoted as $fix(g)$. That is 
    \[fix(g) = \{x \mid g\cdot x = x\}. \]
</div>

<div class='proof' text='Proof of Part 1'>
    Considering the extension of $BC$, we have $2 \alpha + 2 \frac{\angle B}{2} = 180$, and therefore, 
    \[ \alpha + \frac{\angle B}{2} = 90^\circ.\]
    That is $$\angle I_CBI = \angle{IBI_A} = 90^\circ.$$
    This implies that $I_C, B, I_A$ are collinear. Also, $I_B \exists  \angle{B} \text{ bisector}$. Therefore, $I_BB\perp I_CI_A$.
</div>

## Miscellaneous
### Show / Hide
```md
<div class='hidden' desc='Hidden Text'>
Some hidden stuff goes here.
$$\begin{align}
a^3 &= b^2 - c^5, \\\\
b^0 &= \log(2^5).
\end{align}$$
</div>
```
<div class='hidden' desc='Hidden Text'>
Some hidden stuff goes here.
$$\begin{align}
a^3 &= b^2 - c^5, \\\\
b^0 &= \log(2^5).
\end{align}$$
</div>

```md
Here is an example of <span class='hidden' desc='hidden inline'>$a^2 + b^2 =5$</span> text. 
continuation follows.
```
Here is an example of <span class='hidden' desc='hidden inline'>$a^2 + b^2 =5$</span> text. continuation follows.

This is a test of how to include a problem solution. 

<div class='problem' text='IMO 2021/5'>
Two squirrels, Bushy and Jumpy, have collected 2021 walnuts for the winter. Jumpy numbers the walnuts from 1 through 2021, and digs 2021 little holes in a circular pattern in the ground around their favourite tree. The next morning Jumpy notices that Bushy had placed one walnut into each hole, but had paid no attention to the numbering. Unhappy, Jumpy decides to reorder the walnuts by performing a sequence of 2021 moves. In the $k$-th move, Jumpy swaps the positions of the two walnuts adjacent to walnut $k$.

Prove that there exists a value of $k$ such that, on the $k$-th move, Jumpy swaps some walnuts $a$ and $b$ such that $a < k < b$.
</div>

<div class='hidden' desc='Solution'>
This is where to input a solution. 

<div class='claim-un'>
It is possible to use claims inside hidden text.
</div>

<div class='proof'>
See the above text. 
</div>
</div>

<div class='remark'>
Unnumbered claims also exist. 
</div>

### Code Blocks

#### Asy
Use either `c` or `c++`.
```c++
unitsize(1cm);
int pth[] = {0,1,0,1,1,1,0,1};

for (int x = 0; x <= 10; ++x)
for (int y = 0; y <= 6; ++y) {
    draw((0,y)--(10,y)^^(x,0)--(x,6), gray(0.75));
}
```
#### Python
```python
def mex(mex_set):
    ret = 0
    while ret in mex_set:
        ret += 1
    return ret
```

#### Latex
```tex
\section{Section Two}
\begin{enumerate}[(\Roman*)]
    \item First
    \item Second
\end{enumerate}
```
#### Ruby
```ruby
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
```
