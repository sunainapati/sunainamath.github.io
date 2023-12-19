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
Let $ABC$ be a triangle. The incircle of $ABC$ has center $I$ and is tangent to $AB$
and $AC$ at $D$ and $E$ respectively. Let $O$ denote the circumcenter of $BCI$. Prove
that $\angle ODB = \angle OEC$.
</div>
<div class='proof'>
Note that $A,I,O$ are collinear. Now $$\triangle ADO \cong \triangle AEO \implies \angle ODB = \angle OEC$$ 
</div>

<div class='example' text='USAJMO 2020/4'>
Let $ABCD$ be a convex quadrilateral inscribed in a circle and satisfying $DA < AB = BC < CD$. Points $E$ and $F$ are chosen on sides $CD$ and $AB$ such that $BE \perp AC$ and $EF \parallel BC$. Prove that $FB = FD$.
</div>
<div class='proof'>
Let $P = AC \cap BE$. Since $\triangle{ABC}$ is isosceles we know that $P$ is the mid point of $AC$. Let $\angle{CBE} = \angle{ABE} = \alpha$. We also know that $\angle{BCA} = \angle{BAC} = 90 - \alpha$. By parallel lines we know that $\angle{FEB} = \alpha$. Hence $\triangle{FEB}$ is isosceles or $FB = FE$.

Let $\angle{DCA} = \angle{DBA} = \theta$. By parallel lines we see that $\angle{DEF} = 90 - \alpha + \theta$. Since $EP \perp AC$ and $P$ is the midpoint of $AC$ as previously stated, we know that $\triangle{AEC}$ is isosceles or $\angle{EAC} = \angle{ECA} = \theta$.

Note that $AFED$ is cyclic due to\[\angle{AFE} + \angle{ADE} = 180 - \angle{BFE} + 180 - \angle{ABC} = 180 - (180 - 2\alpha) + 180 - 2\alpha = 180.\]Hence we know that $\angle{FAE} = \angle{FAC} + \angle{CAE} = 90 - \alpha + \theta = \angle{FDE}$ meaning that $\angle{FDE} = \angle{FED}$ or $\triangle{FED}$ is isosceles.

Therefore we know that $FE = FD$. Previously we found that $FB = FE$, thus we get $FB = FE$ as desired.
</div>

<div class='example' text='IMO 2000/1'>
Two circles $G_1$ and $G_2$ intersect at two points $M$ and $N$. Let $AB$ be the line tangent to these circles at $A$ and $B$,
respectively, so that $M$ lies closer to $AB$ than $N$. Let $CD$ be the line parallel to $AB$
and passing through the point $M$, with $C$ on $G_1$ and $D$ on $G_2$. Lines $AC$ and $BD$ meet at $E$; lines $AN$ and $CD$ meet at $P$;
lines $BN$ and $CD$ meet at $Q$. Show that $EP = EQ$.
</div>
<div class='proof'>
Let $MN\cap AB=P \implies M$ is midpoint of $PQ.$  It is enough to show that $EM\cap CD$ or show that $EM\cap AB.$ Note that $$\angle ACM=\angle,~~\angle EAB=\angle ECD.$$ So $EAMB$ is kite. And we are done.
</div>

<div class='example' text='2019/G1'>
Let $ABC$ be a triangle. Circle $\Gamma$ passes through $A$, meets segments $AB$ and $AC$ again at points $D$ and $E$ respectively, and intersects segment $BC$ at $F$ and $G$ such that $F$ lies between $B$ and $G$. The tangent to circle $BDF$ at $F$ and the tangent to circle $CEG$ at $G$ meet at point $T$. Suppose that points $A$ and $T$ are distinct. Prove that line $AT$ is parallel to $BC$.

</div>
<div class='proof'>
Redefine $T$ such that $T\in (ABC)$ and $AT||BC$.
<div class='claim'>
  $TF$ tangent to $(BDF)$.
</div>
  <div class='proof'>
    Note that is enough to show that $180-\angle BDF=\angle BFT$. But note that$$\angle BDF=\angle TFG=\angle FTA.$$
  </div>
Similarly, we get that $TG$ is tangent to $(EGC)$. And we are done.
</div>

<div class='example' text='EGMO 2016/P4'>
Two circles $\omega_1$ and $\omega_2$, of equal radius intersect at different points $X_1$ and $X_2$.
Consider a circle $\omega$ externally tangent to $\omega_1$ at $T_1$ and internally tangent to $\omega_2$ at point $T_2$.
Prove that lines $X_1T_1$ and $X_2T_2$ intersect at a point lying on $\omega$.
</div>
<div class='proof'>
Note that the composition of homotheties gives us$$ \omega_1 \xrightarrow{T_1} \omega \xrightarrow{T_2} \omega_2. $$Moreover, since the product of scales are $-1$ ( not $1$, else it will be a transformation), so the composition is a homothety.

But the homothety taking $\omega_1\rightarrow \omega_2$ is simply $1$ or $-1$ ratio as the radius is the same and the centre lies on $O_1O_2$. But ratio $1$ is absurd. Hence,the ratio is $-1$ with the centre of the homothety being the midpoint of $X_1X_2,O_1O_2$.

Let $M$ be the midpoint of $O_1O_2,X_1X_2$. So note that$$\omega_1\xrightarrow{O} \omega_2=\omega_1 \xrightarrow{T_1} \omega \xrightarrow{T_2} \omega_2.$$But the homothety $\omega_1\xrightarrow{O} \omega_2$ takes $X_1\rightarrow X_2$. Now, we consider the homothety $\omega_1 \xrightarrow{T_1} \omega \xrightarrow{T_2} \omega_2$, this takes$$X_1\rightarrow X_1T_1\cap \omega \text { say } A \rightarrow AT_2\cap \omega_2.$$But we should have $AT_2\cap \omega_2=X_2$. So $T_2-A-X_2$. And we are done!
</div>

<div class='example' text='EGMO 2012 P1'>
Let $ABC$ be a triangle with circumcentre $O$. The points $D,E,F$ lie in the interiors of the sides $BC,CA,AB$ respectively, such that $DE$ is perpendicular to $CO$ and $DF$ is perpendicular to $BO$. (By interior we mean, for example, that the point $D$ lies on the line $BC$ and $D$ is between $B$ and $C$ on that line.)
Let $K$ be the circumcentre of triangle $AFE$. Prove that the lines $DK$ and $BC$ are perpendicular.
</div>
<div class='proof'>
Note that $\angle FKE=2\angle A$ and$$\angle OBC=\angle OCB=90-\angle A\implies \angle FDB=\angle EDC=A\implies \angle FDE=180-2\angle A\implies KFDE \text{ cyclic}.$$
As$$KF=KE\implies \angle KEF=90-A\implies \angle KDF=90-A\implies $$$$\angle KDB=\angle KDF+\angle FDB=90$$$$\implies KD\perp BC.$$And we are done.
</div>

<div class='example' text='IMO 2023 P2'>
Let $ABC$ be an acute-angled triangle with $AB\le AC$. Let $\Omega$ be the circumcircle of $ABC$. Let $S$ be the midpoint of the arc $CB$ of $\Omega$ containing $A$. The perpendicular from $A$ to $BC$ meets $BS$ at $D$ and meets $\Omega$ again at $E \neq A$. The line through $D$ parallel to $BC$ meets line $BE$ at $L$. Denote the circumcircle of triangle $BDL$ by $\omega$. Let $\omega$ meet $\Omega$ again at $P \neq B$. Prove that the line tangent to $\omega$ at $P$ meets line $BS$ on the internal angle bisector of $\angle BAC$.


</div>
<div class='proof'>
Define $A'$ as the antipode of $A$. And redefine $P=A'D\cap (ABC)$. Define $L=SP\cap (PDB)$. 
<div class='claim'>
   $L-B-E$ collinear
</div>
<div class='proof'>
  Note that $$\angle SCA=\angle SCB-\angle ACB=90-A/2-C.$$
So $$\angle SPA=90-A/2-C\implies \angle SPA'=90-(90-A/2-C)=A/2+C\implies \angle LBD=A/2+C\implies \angle LBD=A/2+C.$$
By angle chase, $$\angle DBC=90-A/2,\angle EBC=90-C.$$ So $E-B-L$ collinear.
</div>
  
<div class='claim'>
  $LD||BC$
</div>
<div class='proof'>
  Define $F$ as midpoint of arc $BC$ not containing $A$.
Now define $X=PP\cap AF$. Define $O$ as the circumcenter of $(ABC)$. 
We know that $$\angle EBC=90-C,\angle ELD=\angle BLD=\angle BPD=\angle BPA'=\angle BAO=90-C.$$
So $LD||BC$.
  
</div>
<div class='claim'>
  $PXOF$ is cyclic
</div>
<div class='proof'>
   Let $\angle PAB=\theta$. So $\angle PSB=\theta$ and $\angle PSF=\theta+A/2$. So $\angle POF=2\theta+A$. 
And $\angle PXF=\angle PAX+\angle APX$. But $\angle PAX=\theta+A/2$. And $$\angle APX=\angle APS+\angle SPX=\angle ACS+\angle SPX=90-A/2-C+\angle SPX.$$
So to show cyclicity, we need to show that $$2\theta+A=\angle PXF=90+\theta-C+\angle SPX.$$
Or enough to show $$\angle SPX=\theta+A-90+C.$$
But $$\angle SPX=\angle SPB-\angle XPB$$ 
$$=\angle SAB-\angle XPD-\angle DPB= 90+A/2-\angle DBP-\angle DLB$$
$$=90+A/2-\angle DLP-(90-C)$$
$$=C+A/2-\angle DLP$$
as $SF||AD,BC||LD, AD\perp BC$ we get $$C+A/2-\angle DLP=C+A/2-(90-A/2-\theta)=C+A-90+\theta.$$
And so we get $PXOF$ is cyclic.
</div>
<div class='claim'>
  $XA=XP$
</div>
<div class='proof'>
  Note that $$\angle XPA=\angle PXF-\angle PAX=2\theta+A-\theta-A/2=\theta+A/2$$. So $\angle XPA=\angle XAP$. And hence the claim.
But $$XA^2=XP^2=XD\cdot XB.$$ So $XA$ is tangent to $(DBA)$. Hence $$\angle ABD=\angle DAS=\angle DAF=\angle AFS=\angle ABS.$$

</div>
And hence we get $B-X-S$ collinear.

And we are done! 
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



