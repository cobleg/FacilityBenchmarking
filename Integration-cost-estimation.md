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
Integration cost can be quantified through the combination of:
- screening curves
- load duration curve

### Screening curves
Screening curves define the annual cost of facilities by technology over the period of a full year

$$
C_{y,i}=FC_{i} \times CRF+ FOM_{i}+VC_{y,i} \times FLH_{i}
$$
where
$FC_i$ is the fixed cost of technology $i$
$CRF$ is an amortisation factor
$FOM_i$ is the fixed operating and maintenance cost for technology $i$
$VC_{y,i}$ is the variable cost of in year $y$ for technology $i$ 
$FLH_i$ is the full-load hour output for technology $i$

[@pratamaScreeningCurveValuing2021]





## Decomposing integration cost


# References
