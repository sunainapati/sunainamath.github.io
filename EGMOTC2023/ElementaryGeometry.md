---
layout: post
_title: EGMOTC 2023 Elementary Geometry 
---

Firstly, welcome to European Girls' Mathematical Olympiad Training camp 2023!I am so happy for all of you and very excited to teach all of you. 

Elementary Geometry doesn't have any prerequisite. So do not be scared. And now, let's try to do some maths!

I will be using Kenneth Peng's Geometry Through Problems as the main reference for the classes. 

<div class='example'>
  Let $ABCD$ be a quadrilateral. Let $M,N,P,Q$ be the midpoints of sides $AB,BC,CD,DA$. Prove that $MNPQ$ is a parallelogram.
</div>
<div class='proof'>
  Consider $\Delta ABD$ and  $\Delta BDC$ .Note that $NP||BD||MQ$. Similarly, $NM||AC||PQ$. Hence the parallelogram.
</div>

<div class='example'>
 In $\Delta ABC$, $\angle A$ be right. Let $D$ be the foot of the altitude from $A$ onto $BC$. Prove that $AD^2=BD\cdot CD$.
</div>
<div class='proof'>
  Note that $\Delta ADB\sim \Delta CDA$. So by similarity, we have $$\frac{AD}{BD}=\frac{CD}{AD}.$$
</div>

<div class='example' text='Angle Bisector Theorem'>
 In $\Delta ABC$, $\angle A$ be right. Let $D$ be the foot of the altitude from $A$ onto $BC$. Prove that $AD^2=BD\cdot CD$.
</div>
<div class='proof'>
  Let $D\in CA$, such that $AD = AB$.Note that $BD||AS$. So by the Thales’ Proportionality Theorem, we are done!
</div>

<div class='example'>
Given $\Delta ABC$, construct equilateral triangles $\Delta BCD,\Delta CAE,\Delta ABF$ outside of $\Delta ABC$. Prove that $AD=BE=CF$.
</div>
<div class='proof'>
This is just congruence. Note that in $\Delta ABD, \Delta FBC$ we have $$\angle FBC=\angle ABC+60^{\circ}=\angle ABD.$$ And $FB=AB,BC=BD$. So we get $\Delta ABD \cong \Delta FBC$. So $AD=FC$. Similarly, we can show $BE=FC$.
</div>

<div class='example' text='Menelaus Theorem'>
If line $PQ$ intersecting $AB$ on $\triangle ABC$, where $P$ is on $BC$, $Q$ is on the extension of $AC$, and $R$ on the intersection of $PQ$ and $AB$, then\[\frac{PB}{CP} \cdot \frac{QC}{QA} \cdot \frac{AR}{RB} = 1.\]
</div>
<div class='proof'>
Draw a line parallel to $QP$ through $A$ to intersect $BC$ at $K$.
$$\triangle RBP \sim \triangle ABK \implies \frac{AR}{RB}=\frac{KP}{PB}$$
$$\triangle QCP \sim \triangle ACK \implies \frac{QC}{QA}=\frac{CP}{KP}$$
Multiplying the two equalities together to eliminate the $PK$ factor, we get:
$\frac{AR}{RB}\cdot\frac{QC}{QA}=\frac{CP}{PB}\implies \frac{AR}{RB}\cdot\frac{QC}{QA}\cdot\frac{PB}{CP}=1$
</div>

<div class='example' text='Miquels Theorem'>
In $\Delta ABC$, choose points $D,E,F$ on sides $BC,CA,AB$ respectively. Prove that circles $(AEF),(BFD),(CDE)$ share a point known as the miquel point. 
</div>
<div class='proof'>
Define $M=(AEF)\cap (BFD)$. So note that $$\measuredangle FME=\measuredangle A,\measuredangle EMD=\measuredangle C\implies \measuredangle FMD=B\implies M\in (DFB).$$
</div>

<div class='example' text='Reims Theorem'>
Let $\omega_1, \omega_2$ be two circles intersecting at $M,N$. Let line $\ell_M$ through $M$ intersect $\omega_1, \omega_2$ at $A_1, A_2$. Let $B_1, B_2$ be points on $\omega_1, \omega_2$ respectively, Then $A_1B_1\parallel A_2B_2$ if , and only if, $B_1,N,B_2$ are collinear on a line $\ell_N$.
</div>
<div class='proof'>
Suppose that B_1NB_2 is a straight line. Then $$\measuredangle MA_1B_1 = \measuredangle MNB_1 = \measuredangle MA_2B_2 \implies A_1B_1 \parallel A_2B_2.$$
</div>

<div class='example' text='Simson Line'>
Let a triangle $\triangle ABC$ and a point $P$ be given. Let $D, E,$ and $F$ be the foots of the perpendiculars dropped from P to lines AB, AC, and BC, respectively. Then points $D, E,$ and $F$ are collinear iff the point $P$ lies on circumcircle of $\triangle ABC.$
</div>
<div class='proof'>
Let the point $P$ be on the circumcircle of $\triangle ABC.$ So $$\angle BFP = \angle BDP = 90^\circ \implies BPDF \text{ is cyclic }\implies \angle PDF = 180^\circ – \angle CBP.$$
So $$\angle ADP = \angle AEP = 90^\circ \implies AEPD \text{ is cyclic }$\implies \angle PDE = \angle PAE.$$
And $$ACBP \text{ is cyclic } \implies \angle PBC = \angle PAE \implies \angle PDF + \angle PDE = 180^\circ$$
$\implies D, E,$ and $F$ are collinear as desired.
</div>

<div class='example' text=''>
Let $AB$ be a chord in $\omega(O, r)$ and let $TA$ be a tangent to $\omega$ at $A$. Let $\angle BAT = \alpha$. Let $\angle APB$ be any inscribed angle over the arc $AB$. Then $$\angle BAT=\angle APB.$$
</div>
<div class='proof'>
Since $TA$ is a tangent, then it must be perpendicular to $OA$. So  $\angle OAT = 90^{\circ}$. So $\angle OAB = \angle OAT − \angle BAT = 90− \alpha$. 
Note that $\Delta OAB$ is isosceles. So  $$\angle OAB = \angle OBA = 90^{\circ} − \alpha,\angle AOB = 180^{\circ} −2(90^{\circ} −\alpha) = 2\alpha.$$ And $\angle APB=\angle AOB/2=\alpha$. So done.
</div>

## Olympiad Problems 
<div class='example' text='STEMS 2024, CAT A, P3'>
Let $ABC$ be a triangle. Let $I$ be the Incenter of $ABC$ and $S$ be the midpoint of arc $BAC$. Define $IA$ as the $A$-excenter wrt $ABC$. Define $\omega$ to be the circle centred at $S$ with radius $SB$. Let $AI_A \cap \omega = X$, $Y$. Show that $\angle BCX = \angle ACY$.
</div>
<div class='proof'>
 Note that$$\angle AYC=\angle XYC=\angle XBC.$$And we have$$\angle BXC=180-\frac{BSC}{2} = 180 - \frac{A}{2}.$$And note that $X-A-Y$ is the angle bisector of $\angle BAC$. So$$\angle YAC=180-\frac{A}{2}.$$So we get that$$\Delta BXC\sim\Delta YAC\implies \angle BCX=\angle ACY.$$
</div>
<div class='example' text=''>

</div>
<div class='proof'>

</div>

<div class='example' text=''>

</div>
<div class='proof'>

</div>

<div class='example' text=''>

</div>
<div class='proof'>

</div>

<div class='example' text=''>

</div>
<div class='proof'>

</div>

<div class='example' text=''>

</div>
<div class='proof'>

</div>

<div class='example' text=''>

</div>
<div class='proof'>

</div>

<div class='example' text=''>

</div>
<div class='proof'>

</div>

<div class='example' text=''>

</div>
<div class='proof'>

</div>

<div class='example' text=''>

</div>
<div class='proof'>

</div>

<div class='example' text=''>

</div>
<div class='proof'>

</div>

<div class='example' text=''>

</div>
<div class='proof'>

</div>

<div class='example' text=''>

</div>
<div class='proof'>

</div>

<div class='example' text=''>

</div>
<div class='proof'>

</div>

<div class='example' text=''>

</div>
<div class='proof'>

</div>

<div class='example' text=''>

</div>
<div class='proof'>

</div>

<div class='example' text=''>

</div>
<div class='proof'>

</div>



