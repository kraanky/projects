<h1 style="text-align: center;"><span style="font-family:Didot; font-size: 24pt; color: #34495e;"><strong>Stoichiometric Coefficients and
Reaction Progress Variables</strong></span></h1>

### Stoichiometric Coefficients
Any arbitrary chemical reaction can be written as:
<p style="text-align:center;">$bB+cC+... = sS+tT+...$</p>
where species B and C are the reactants, species S and T are the products and b, c, s, t are the stoichiometric coefficients (also generalised as $\nu_i$) of  B, C, S and T respectively. 

Conventionally, $\nu_i$ for reactants is negative as reactants are consumed in a reaction. Products are generated in a reaction so $\nu_i$ is positive for products. Non-reacting species have $\nu_i=0.$

By the generalized material balance equation, we arrive at the conclusion:
<p style="text-align:center;">$\nu_BB + \nu_CC + \nu_SS + \nu_TT + ... = 0$</p>
or
<p style="text-align:center;">$\sum_i\nu_iA_i = 0 \tag{1}$</p>
for all components $A_i$ in the system.

Let's take an example:
<p style="text-align:center;">$2CO+O_2 \rightarrow 2CO_2$</p>
This can also be written as:
<p style="text-align:center;">$\ CO+\frac{1}{2}O_2 \rightarrow CO_2$</p>
<p style="text-align:center; font-size: 12pt">$\frac{\nu_{CO}}{\nu_{O_2}} = \frac{-2}{-1}=\frac{-1}{-1/2}=2$</p>

This is an important observation:<i> reactions may be balance differently but the ratio of stoichiometric coefficients stays the same.</i>

### Reaction Progress Variable
Put simply, the amount of reactant consumed in a reaction is the reaction progress variable($\epsilon$) or reaction. Naturally, it is defined as:
<p style="text-align:center;">$\epsilon = \frac{n_i - n_i^0}{\nu_i}\\ n_i = n_i^0 + \nu_i\epsilon \tag{2}$</p>

The above equation is valid for all components in the system. Notice that $\epsilon$ is a time-dependent extensive variable.

Change in moles of two species $i$ and $j$ can be written as:
<p style="text-align:center;">$n_i - n_i^0 = \nu_i\epsilon \\ n_j - n_j^0 = \nu_j\epsilon \\ \Rightarrow \epsilon = \frac{n_i - n_i^0}{\nu_i} = \frac{n_j - n_j^0}{\nu_j}$</p>
<p style="text-align:center;">$n_j - n_j^0 = \frac{\nu_j}{\nu_i}(n_i - n_i^0 ) \tag{3}$</p>

If multiple reactions occur then the $k^{th}$ reaction has reaction coordinate $\epsilon_k$. 
If there are $r$ reactions occurring in a system, the change in moles of species $i$ would be:
<p style="text-align:center;">$n_i - n_i^0 = \sum_k^{k=r} \nu_{ki}\epsilon_k \tag{4}$</p>

This is the sum of amounts of species $i$ consumed or produced in each reaction.

An advantage of this concept is that we can relate concentration of a species with the reaction coordinate which is only related to the reaction conditions. 

A disadvantage of this concept is that $\epsilon$ is an extensive property; it is defined for a closed system and it is proportional to the mass of the mass.

The fraction $f$ is an intensive measure of the progress of the reaction:
<p style="text-align:center;">$f=\frac{change\ in\ moles\ of\ i}{initial\ moles\ of\ i}=\frac{n_i^0-n_i}{n_i^0} = 1-\frac{n_i}{n_i^0}=\frac{-\epsilon\nu_i}{n_i^0} \tag{5}$</p>
<p style="text-align:center;">$0 \leq f \leq 1$</p>

This is a useful concept - if the reaction is not limited by thermodynamic equilibrium constraints then it is limited by the initial moles of the component.

So we can define $f$ in terms of the limiting reactant for calculating the extent of the reaction
$n_{lim} = n_{lim}^0(1-f) \\ = n_{lim}^0 + \nu_{lim}\epsilon \tag{6}$

When multiple reactions take place in a batch reactor, $\epsilon$ (extensive concept) is used.
In an open continuous system such as flow reactors, $f$ (intensive concept) is used.

At equilibrium, $f_e$ is the conversion of the limiting component and $\epsilon_e$ is the extent of the reaction.
<p style="text-align:center;">$\epsilon_e = -\frac{f_e n_{lim}^0}{\nu_{lim}} \label{eq7}\tag{7}$</p>

In some cases, the maximum extent of the reaction is the equilibrium extent of the reaction - this means the reaction highly favors formation of products. These reactions are classified as <i>irreversible</i>.
<p style="text-align:center;">$\epsilon_e \approx \epsilon_{max}\ or\ \frac{\epsilon_e}{\epsilon_{max}} \approx 1$</p>

On the other hand, if $\epsilon_e$ and $\epsilon_{max}$ differ greatly, the reaction is classified as <i>reversible</i>
<p style="text-align:center;">$\frac{\epsilon_e}{\epsilon_{max}} >> 1$</p>

From a thermodynamic point of view, all reactions are reversible but in a reacting system it is convenient to ignore the reverse reaction as its progress coordinate is negligibly small.