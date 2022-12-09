Levelised Cost of Energy (LCoE) is a measure of the averge net present cost of energy that a facility of a specified type will produce over its expected operating life. Think of this as the lifetime unit (or average) cost.

## Formulation
### Standard formulation
The LCoE is calculated as:

Equation 1:

$$
LCoE = \frac{\text{sum of lifetime cost}}{\text{sum of lifetime energy produced}}
$$ 
$$
LCoE = \frac{\Sigma_{t=1}^{n}\frac{I_t+M_t+E_t}{(1+r)^t}}{\Sigma_{t=1}^{n}\frac{O_t}{(1+r)^t}}
$$
[@LevelizedCostElectricity2022]

where
$I_t$ is investment expenditure in year $t$
$M_t$ is operations and maintenance cost in year $t$
$E_t$ is expenditure on primary energy in year $t$
$0 \lt r \le 1$ is the discount rate used to reflect the opportunity cost of waiting
$O_t$ is the output quantity in year $t$
$n$ is the assumed operational lifetime of the facility.

## Implicit assumptions
The apparent simplicity of the LCoE model hides a few important issues:
- Expected utilisation of the facility being modelled
- Learning curve rates associated with nascent technologies
- Economies of scale and/or scope of output
- The facility being modelled is a new facility
- There are no system integration costs.

These assumptions are implicit within the forecast output $O_t$ and some of the cost items such as $I_t$. 
The LCoE is effectively a lifetime unit cost calculation and unit costs are affected by all three implicit assumptions. 

The learning curve effect represents a downward shift of unit cost over its operational lifetime, so timing of investment is critical since it ties a facility to a specific vintage of capital. The presumption being that later vintages of facility technology will imply a lower unit cost and LCoE than the current vintage. For example, photovoltaic panel efficiency is currently 15% to 20% efficient whereas future panel efficiency could be in the 25% to 30% range. This implies a higher yield from future technologies. 

Economies of scale represent a movement along a unit cost curve and is directly tied to both the capacity of the facility typically measured in megawatts (MW) and capacity factor (i.e. utilisation). 

Economies of scope across facilities that provide more than one service may mean that joint production of services results in a lower unit cost as the production of each service increases. 

Facility age affects the maximum output over time. Aged facilities will likely be producing less than the facility did it was initially commissioned. Moreover, the aged facility will be utilising an earlier vintage of technology. For example, an old open cycle gas turbine will have less fuel economy than a more recent vintage.

The underlying facility technologies impose differing cost of system integration. For example, variable renewable energy systems (e.g. photovoltaic and wind power) impose additional contingency reserve costs in electricity systems. The standard LCoE formulation does not recognise this cost. On occasion, LCoE estimates include a penalty cost to correct for this omission. 

## Average versus marginal cost
The prospect of a dynamic unit cost implies that the underlying LCoE assumption of average cost equal to marginal cost is not valid. In using the standard LCoE formulation, the basis of comparison is strictly static. With year-to-year variation in capacity factor, this could restriction could render the analysis useless.

### Increasing share of variable renewable energy facilities
Marginal cost is defined as the change in total cost as output changes.  [@2008InterpretationShort] In an electrical system, a change in the share of variable renewable energy facility production in total system output imposes an incremental cost of integration. This cost of integration implies an additional component of marginal cost. [Marginal cost](Introduction#Marginal cost.md) 

## System LCoE

System LCoE of a technology is defined as the sum of generation costs and integration costs per generation unit from a specific technology (e.g. wind power). [@ueckerdtSystemLCOEWhat2013]

Equation 2:
$$
sLCoE_{vre} = \overline{LCoE}_{vre}+\Delta I
$$
where
$sLCoE_{vre}$ is the system LCoE cost imposed by variable renewable energy systems
$\overline{LCoE}_{vre}$ is the marginal generation cost of variable renewable energy in per-MWh
$I$ is the integration cost

Note that 

Equation 3:
$$
\Delta I = \frac{dC_{integration}}{dE_{vre}}
$$
where
$C_{integration}$ is the cost of integration
$E_{vre}$ is the lifetime electrical power produced by the additional variable renewable energy system

The corresponding lifetime system total cost is

Equation 4:
$$
C_{total}=C_{vre}+C_{residual}
$$
where
$C_{vre}$ is the direct cost of VRE
$C_{residual}$ is the balance of system cost

In the case without VRE, $C_{residual}=0$ and $C_{total}=C_{residual}$.

In the case with VRE capacity greater than zero,  define the cost of VRE integration as the residual cost less the proportion of cost with no VRE system integration

Equation 5 :
$$
C_{integration}=C_{residual}-\frac{E_{residual}}{E_{total}}C_{total}(0)
$$
where
$C_{residual}=C_{total}-C_{vre}$ is the system total cost less the direct cost of variable renewable energy systems
$E_{residual}=E_{total}-E_{vre}$ is the remaining electrical power required to satisfy the demand for electrical power after variable renewable energy systems has exhausted its capacity.
$E_{total}$ is the total electrical power required to satisfy demand
$C_{total}(0)$ is the total system cost with no variable renewable energy capacity.

This definition of the cost of integration permits decomposition of total lieftime system cost (Equation 4) into

Equation 5:
$$
C_{total} = C_{vre} + C_{integration}+\frac{E_{residual}}{E_{total}}C_{total}(0)
$$
Note that by definition of $E_{residual}$, Equation 5 can be restated as

Equation 5a:

$$
C_{total} = C_{vre} + C_{integration}+\frac{E_{total}-E_{vre}}{E_{total}}C_{total}(0)
$$

From Equation 5a observe that a system with no VRE capacity installed has system lifetime total cost

$$
C_{total} = \frac{E_{total}}{E_{total}}C_{total}(0)

$$

The optimal level of variable renewable energy system deployment is determined by minimising total lifetime system cost. The cost minimisation rule implies a first-order change in cost with respect to a small unit change in lifetime VRE output is set equal to zero

Equation 6:
$$
\text{min }C_{total} \implies \frac{dC_{total}}{dE_{vre}}=0
$$

Applying this rule to Equation 5 yields the optimality condition

Equation 7:
$$

\text{min }C_{total} \implies \frac{dC_{vre}}{dE_{vre}}+\frac{dC_{integration}}{dE_{vre}}+\frac{d}{dE_{vre}} \left( \frac{E_{residual}}{E_{total}}C_{total}(0) \right) = 0

$$
In words, this condition states that total lifetime system cost is minimised when the  sum of the marginal lifeetime cost of VRE and the marginal net cost of VRE integration is zero. 

From Equation 5 no VRE implies:

$$
C_{residual}-\frac{E_{residual}}{E_{total}}C_{total}(0)=0
$$
which can be restated as
  
$$
\frac{C_{residual}}{E_{residual}}=\frac{C_{total}(0)}{E_{total}}
$$


Given Equation 5 the corresponding system LCoE equation is

### Deriving system LCoE from total lifetime system cost

Divide total lifetime system cost (Equation 5a) by lifetime total output

$$
\frac{C_{total}}{E_{total}} = \frac{C_{vre}+C_{integration}}{E_{total}} + \frac{E_{total}-E_{vre}}{E_{total}} \times \frac{C_{total}(0)}{E_{total}}
$$

Equation 6:

$$
sLCoE_{total}=sLCoE_{vre}+\Delta I+E_{residual}C_{total}(0)
$$
 

Note that a system without any VRE has a total system cost of

Equation 9:

$$
C_{total}=C_{conventional}
$$
where
$C_{conventional}=C_{total}(0)$

with a corresponding average net present cost of

Equation 10:

$$
sLCoE_{conventional} = \frac{C_{total}(0)}{E_{total}}
$$





As [@ueckerdtSystemLCOEWhat2013] highlights


[@matsuoReDefiningSystemLCOE2022]


## References

“2008 Interpretation of Short Run Marginal Cost - Economic Regulation Authority Western Australia.” n.d. Accessed November 19, 2022. [https://www.erawa.com.au/electricity/wholesale-electricity-market/regulatory-papers/2008-interpretation-of-short-run-marginal-cost](https://www.erawa.com.au/electricity/wholesale-electricity-market/regulatory-papers/2008-interpretation-of-short-run-marginal-cost).

“Levelized Cost of Electricity.” 2022. In _Wikipedia_. [https://en.wikipedia.org/w/index.php?title=Levelized_cost_of_electricity&oldid=1111686277](https://en.wikipedia.org/w/index.php?title=Levelized_cost_of_electricity&oldid=1111686277).

Matsuo, Yuhji. 2022. “Re-Defining System LCOE: Costs and Values of Power Sources.” _Energies_ 15 (18, 18): 6845. [https://doi.org/10.3390/en15186845](https://doi.org/10.3390/en15186845).

Ueckerdt, Falko, Lion Hirth, Gunnar Luderer, and Ottmar Edenhofer. 2013. “System LCOE: What Are the Costs of Variable Renewables?” _Energy_ 63 (December): 61–75. [https://doi.org/10.1016/j.energy.2013.10.072](https://doi.org/10.1016/j.energy.2013.10.072).
