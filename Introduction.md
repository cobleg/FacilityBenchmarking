This notebook contains information related to cost benchmarking of electricity supply facilities such as:
- Hydro power plant
- Solar photovoltaic systems
- Wind power systems
- Battery Energy Storage Systems (BESS)
- Open Cycle Gas Turbine electricity generators

## Motivations for benchmarking
Economic regulators and other stakeholders want to have an independent method of evaluating the price of electricity that consumers pay. In the theory of competitive markets, the price of a good or service is based on:
- the efficient cost of operating a facility and
- a mark-up on cost that represents the normal return on an investment asset.

A benchmark model that is based on this theory will provide be a basis to compare the price being paid by consumers and the underlying cost. Prices that are systematically higher than the efficient cost will likely prompt an investigation to determine the underlying cause.

Investors deciding to purchase or build a facility will want to determine the likely competitiveness of the facility and directly estimate the return on investment. 

## Model design
The precise design of a cost benchmarking model is guided by user's needs. The level of detail required will vary and most will not want a model that is too complex and difficult to understand. The design will likely vary according to user needs:
- Economic regulators: Short-run and long-run marginal cost
- Investors: Project finance
- Levelised Cost of Energy: Policy evaluation of alternative technologies.

### Marginal cost model 
A marginal cost model informs the likely change in price offers presented to an electricity market. The core idea is that the cost of supplying a unit of electrical power varies with the amount of electrical power being supplied. 

#### Short-run marginal cost
For a short-run marginal cost model, only costs that vary with output are included. This will include input cost items such as:
- Variable operating and maintenance cost
- Purchase cost of primary energy
- Start-up and shut-down costs

Various techno-economic parameters are required to translate the input cost into output cost, such as heat rates for various types of fuel-based electricity generation facilities. The level of utilisation and frequency of start-up and shut-down are also relevant.

The main model output is a short-run supply curve.

#### Long-run marginal cost
A long-run marginal cost model includes the efficient total cost of building and operating a facility over the expected operating life of the facility. The qualifier `efficient` signifies that any cost deemed not essential to installing and preparing a facility for operation is to be excluded. The most likely candidate for exclusion is corporate overhead cost.

The expected return on capital will also be included in long-run marginal cost based on reference to the expected yield of existing assets that present a similar risk-return profile compared to the facility being modelled.

The main output is a long-run supply curve

### Project finance cost model
The focus of a project finance cost model is to identify the expected return from the facility and its risk profile. The risk profile will encompass elements such as:
- Variation of input cost over the operating life of the facility
- Variation in output cost
- Variation in facility output under a alternative scenarios typically related to market competition and weather conditions.
- Risk of technological obsolescence, which threatens to truncate the profitable life of the facility

The main output is an expected total return on asset with a confidence interval under alternative scenarios. Scenarios typically represent low, medium and high demand for the facility output.

### Levelised cost of energy
Levelised cost of energy ([LCoE](LCoE.md)) is typically used by policy makers and market analysts that need a way of creating a cost ranking alternative facilities that produce energy. This may be used as part of a multi-criteria analysis in which policy makers are considering a range of trade-offs between policy objectives.

LCoE provides a basis for comparison that smoothes out the lumpy costs that can occur when a facility is being constructed or installed as well as varying expected operating lives and levels of utilisation.

The main output of an average cost of output over a specified time interval. 

