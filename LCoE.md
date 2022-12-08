Levelised Cost of Energy (LCoE) is a measure of the averge net present cost of energy that a facility of a specified type will produce over its expected operating life.

## Formulation
The LCoE is calculated as:

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
- The facility being modelled is a new facility.

These assumptions are implicit within the forecast output $O_t$ and some of the cost items such as $I_t$. 
The LCoE is effectively a lifetime unit cost calculation and unit costs are affected by all three implicit assumptions. 

The learning curve effect represents a downward shift of unit cost over its operational lifetime, so timing of investment is critical since it ties a facility to a specific vintage of capital. The presumption being that later vintages of facility technology will imply a lower unit cost and LCoE than the current vintage. For example, photovoltaic panel efficiency is currently 15% to 20% efficient whereas future panel efficiency could be in the 25% to 30% range. This implies a higher yield from future technologies. 

Economies of scale represent a movement along a unit cost curve and is directly tied to both the capacity of the facility typically measured in megawatts (MW) and capacity factor (i.e. utilisation). 

Economies of scope across facilities that provide more than one service may mean that joint production of services results in a lower unit cost as the production of each service increases. 

Facility age affects the maximum output over time. Aged facilities will likely be producing less than the facility did it was initially commissioned. Moreover, the aged facility will be utilising an earlier vintage of technology. For example, an old open cycle gas turbine will have less fuel economy than a more recent vintage.

## Average versus marginal cost
The prospect of a dynamic unit cost implies that the underlying LCoE assumption of average cost equal to marginal cost is not valid. In using the standard LCoE formulation, the basis of comparison is strictly static. With year-to-year variation in capacity factor, this could restriction could render the analysis useless.

### Increasing share of variable renewable energy facilities
Marginal cost is defined as the change in total cost as output changes.  [@2008InterpretationShort] In an electrical system, a change in the share of variable renewable energy facility production in total system output imposes an incremental cost of integration. This cost of integration implies an additional component of marginal cost. [Marginal cost](Introduction#Marginal cost.md) 



## References

“2008 Interpretation of Short Run Marginal Cost - Economic Regulation Authority Western Australia.” n.d. Accessed November 19, 2022. [https://www.erawa.com.au/electricity/wholesale-electricity-market/regulatory-papers/2008-interpretation-of-short-run-marginal-cost](https://www.erawa.com.au/electricity/wholesale-electricity-market/regulatory-papers/2008-interpretation-of-short-run-marginal-cost).

“Levelized Cost of Electricity.” 2022. In _Wikipedia_. [https://en.wikipedia.org/w/index.php?title=Levelized_cost_of_electricity&oldid=1111686277](https://en.wikipedia.org/w/index.php?title=Levelized_cost_of_electricity&oldid=1111686277).
