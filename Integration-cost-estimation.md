Estimating the integration cost of variable renewable energy (VRE) systems requires the use of a benchmark. Specifically, two cases are defined:
1. Case 1: A system without VRE systems
2. Case 2: A system with VRE systems

Calculating the difference in total cost between Case 2 and Case 1 isolates the total integration cost.

The benchark is based on the residual cost as defined in the [LCoE](LCoE.md) note applied to a technology that does not impose integration costs.

$$
C_{residual}^{BM}=\frac{E_{residual}}{E_{total}}C_{total}(0)
$$
where
$E_{residual}$ is the component of electrical power that is not supplied by VRE systems
$E_{total}$ is the total electrical power supplied
$C_{total}(0)$ is the total lifetime system cost without VRE systems
[@ueckerdtSystemLCOEWhat2013]

Note that the integration cost of VRE is the additional cost in the residual power system that VRE impose compared to the benchmark.

$$
C_{integration}=C_{residual}-C_{residual}^{BM}
$$

The method to estimation of integration cost is to use a simulation model that compares a power system across Case 1 and Case 2 as defined above.

## Quantifying integration costs
Integration cost can be quantified through the combination of the following functions:
- screening curves
- reverse load duration curve

The key steps for this procedure are:
1. Calculate the normalised screening curves for each electricity supply technology deployed in a specified electricity system. The normalised screening curve is in unit cost terms. For example, unit cost of $/kW
2. Calculate the reverse load duration curve for the electricity system specified in step 1
3. Calculate the intersection point coordinates between each pair of screening curves, segment the reverse load duration curve according to the hour coordinate of each intersection pair
4. For each segment of the reverse load duration curve, create a rank order list of the deployed technology from lowest cost to highest cost
5. Choose the lowest cost technology defined in the screening curve order as defined in step 4
6. Calculate the residual reverse load duration curve as the difference between the reverse load duration curve and the full-load hour quantity of the lowest cost technology 
7. Remove the lowest cost technology from the rank order list defined in step 3
8. Repeat steps 4 to 6 (inclusive) until all of the reverse load area curve is allocated across technologies for each segment of the reverse load duration curve.
9. Calculate the total system cost as the sum product of the screening cost 

The total integration cost is the difference between the total system cost with non-firm technology less the total system cost without the non-firm technology. 

$$
C_{integration}=\Sigma_{i,y} C_{i,y} \times Q_{i,y}
$$
where 
$C_{i,y}$ is the normalised screening cost for technology $i$ in year $y$ 
$Q_{i,y}$ is the demand for electrical power supplied by technology $i$ in year $y$ 

Note that the year subscript recognises the age and vintage of the technologies deployed in the electrical power system in a given year. The underlying assumptions are:
1. That efficiency increases over successive vintages of each technology.
2. Efficiency decreases with age of facilities of each technology type with different rates of degradation across technologies.

### Screening curves
Screening curves define the annual cost of facilities by `firm technology` over the period of a full year

$$
C_{i,y}=FC_{i} \times CRF_{i}+ FOM_{i}+VC_{i,y} \times FLH_{i}
$$
where
$FC_i$ is the fixed cost of technology $i$ given an assumed capacity
$CRF_{i}$ is an amortisation factor determined by the expected operational life of a facility of a specified technology. This is sometimes named the: carrying charge
$FOM_i$ is the fixed operating and maintenance cost for technology $i$
$VC_{y,i}$ is the variable cost of in year $y$ for technology $i$ 
$FLH_i= CF_{i,y} \times 8760$  is the full-load hour output for technology $i$ where $CF$ is capacity factor 

Screening curves for non-firm technology are calculated using a modified form of the firm technology screening curve equation

$$
C_{i,y}=FC_{i} \times \frac{CRF_{i}}{ECF_{i}}+ FOM_{i}+VC_{i,y} \times FLH_{i}
$$
where
$ECF_{i} \le 1$ is the effective capacity factor for technology $i$ 

A low value of $ECF$ amplifies the fixed cost component more than a high value of $ECF$

[@pratamaScreeningCurveValuing2021]

### Load duration curve and reverse load duration curve
A load duration curve is a set ordered pairs of hours and demand for electrical power in order from highest demand to the lowest over a standard calendar year (i.e. 8,760 hours). This defines demand as a function of time such that $t=\{1,2,3,...,8760\}$. 

A reverse load duration curve defines a set of order pairs of hours and demand from lowest demand to highest demand. 

## Decomposing integration cost
 

# References
Pratama, Yoga W., and Niall Mac Dowell. 2021. “Screening Curve for Valuing Power Generation and Storage Technologies in the 21st Century Grid.” SSRN Scholarly Paper. Rochester, NY. [https://doi.org/10.2139/ssrn.3821841](https://doi.org/10.2139/ssrn.3821841).

Ueckerdt, Falko, Lion Hirth, Gunnar Luderer, and Ottmar Edenhofer. 2013. “System LCOE: What Are the Costs of Variable Renewables?” _Energy_ 63 (December): 61–75. [https://doi.org/10.1016/j.energy.2013.10.072](https://doi.org/10.1016/j.energy.2013.10.072).