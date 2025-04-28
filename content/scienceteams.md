---
header_menu: false
---

# Science Teams

Across the different nodes participants will be setting up science teams. These teams will address specific topics as proposed by the team lead, and attempt to engage others in joint analysis. These are open for participants at all nodes to join.

Science teams are given a unique identifier (uid) following the convention ‘hk25-uid’. Each team will also have a lead and an associated repo on github with the same uid. The repo will serve as the primary basis for communication among team members.  Mattermost channels, markdown pads, and video-conference links may also serve as supplemental forms of communications, as indicated on by the README for each team.

{{< toc >}}

---
### Energetics of tropical rainbelts ([hk25-RainBelt](https://github.com/digital-earths-global-hackathon/hk25-teams/tree/main/hk25-RainBelt))

Global km-scale grids permits an explicit representation of convective storms and the processes they entails. Over the tropical ocean, precipitation occurs in a variety of environments. Precipitating regions could be related to strong sea surface temperature gradients and a bottom-heavy circulation (e.g., Eastern Pacific) or a top-heavy circulation, weak SST gradients, and light winds (e.g., Western Pacific). Due to the diversity of pathways in which precipitation occurs, we will analyze how convection is represented across the tropical oceans in the different participating km-scale models using an energetic-moisture framework.

**Coordination**: Hans Segura Cajachagua (hans.segura@mpimet.mpg.de)

#### Sketch of initial activities
* identify the tropical rainbelt
* calculate the entropy forcing and the net precipitation flux at the surface
* compute the type of circulation (top- or bottom-heavy) in the tropical rainbelt
* extract the spectrum of convective coupled equatorial waves

---
### Precipitation over ice-sheets ([hk25-IceSheet](https://github.com/digital-earths-global-hackathon/hk25-teams/tree/main/hk25-IceSheet))

Mass loss of the Greenland and Antarctic ice sheets is an important contributor for current and future sea level rise. To properly drive the surface mass balance calculations in ice sheet models, a realistic simulation of precipitation and surface temperatures is crucial. Regional modeling studies suggest that higher resolution of the atmospheric models driving ice sheet models improves the simulation of processes occurring at the steep margins of the ice sheets, making km-scale global models a promising tool for future coupled atmosphere-ocean-ice sheet modelling as planned for example in the [TerraDT](https://terradt.eu/) project.

In this team we want to compare the simulated surface meteorology over Greenland and Antarctica for participating models and with reanalysis data and observations to assess how suited the models are to drive ice-sheet models.

**Coordination**: Hauke Schmidt (hauke.schmidt@mpimet.mpg.de)

#### Sketch of initial activities:
*	extract model output for the Greenland and Antarctic ice sheets
*	produce precipitation and temperature maps
*	compare annual cycles for regional means and selected locations

---
### Triggering of deep convection ([hk25-ConvTrig](https://github.com/digital-earths-global-hackathon/hk25-teams/tree/main/hk25-ConvTrig))

Convective precipitation within the tropical rainbelts is primarily driven by convective storms.  To better understand the tropical rainbelts as a whole, we want to understand the details of individual convective systems.  An important aspect of individual convective systems is their triggering.  Limited observations and idealized modeling suggest that SST-driven mesoscale boundary layer wind convergence may play a key role in triggering deep convection over tropical oceans, but details are still poorly understood. Km-scale models, which allow an explicit representation of deep convection, are a promising tool to overcome this limited understanding.

In this team, we will test the hypothesis that MCSs over tropical oceans are triggered by mesoscale wind convergence. If possible, we will also look at how mesoscale surface wind convergence depends on mesoscale SST properties.

**Coordination**: Henning Franke (henning.franke@mpimet.mpg.de)

#### Sketch of initial activities
* MCS tracking (together with science teams from other nodes)
* Determine time and location of MCS triggering from MCS tracking results
* Calculate mesoscale surface wind convergence at MCS triggering locations
* Calculate SST gradients and Laplacian.

---
### EarthCARE-Curtains ([hk25-Curtains](https://github.com/digital-earths-global-hackathon/hk25-teams/tree/main/hk25-Curtains))

The goal of this working group is to evaluate the models’ capability of capturing the correct vertical structure of clouds around the globe.

To this end, we propose to extract “virtual curtains” from the simulations alongside the EarthCARE satellite tracks “Curtains" refers to the shape of the dataset, a vertical veil unfolding under the satellite, while “virtual" refers to projection of these 2025 orbit tracks onto the simulated year 2020. Practically, we anticipate to use the upcoming EarthCARE's L2-products for the month of April 2025. We will therefore compare these with all virtual curtains extracted from April month, using a bulk statistical approach. Further, we intend to use the satellite product emulator PAMTRA to convert the model’s output into comparable products such as radar reflectivity. An example of such curtain extraction and conversion is presented in Fig. 2.

**Note:** This science team will closely coordinate with the EarthCARE [cross-cutting](./crosscutting.md) activity.

**Coordination**: Romain Fiévet (romain.fievet@mpimet.mpg.de)

#### Sketch of initial activities
* Recover the EC product and orbital tracks
* Extract the virtual curtain from the models
* Convert these using PAMTRA
* Compare and evaluate the models biases


---
### MCS tracking ([hk25-MCS](https://github.com/digital-earths-global-hackathon/hk25-teams/tree/main/hk25-MCS))

Convective storms, especially those that develop into mesoscale convective systems (MCSs), play a crucial role in producing rainfall and hazardous weather across the globe. While recent studies have shown that DYAMOND models can capture certain aspects of tropical MCSs, such as their frequency and diurnal cycle, significant challenges remain. In particular, accurately representing the distribution of precipitation and its relationship with the surrounding environment continues to be a major hurdle ([Su et al. 2022](https://doi.org/10.2151/jmsj.2022-033); [Feng et al. 2023](https://doi.org/10.1029/2022GL102603); [Song et al. 2024](https://doi.org/10.1029/2024GL109945); [Feng et al. 2024](https://doi.org/10.22541/essoar.172405876.67413040/v1)).

Previous DYAMOND phases provided two 40-day simulation periods for summer and winter, limiting the statistical robustness of model evaluations. The WCRP Digital Earth Global Hackathon will extend these simulations to a full year using multiple global kilometer-scale models, creating an unprecedented opportunity to assess how well they capture the full spectrum of convective storms and extreme events. As part of this effort, we are organizing an MCS tracking activity to develop and apply new analysis tools, exchange insights, and strengthen collaborations within the broader atmospheric science community.

**Coordination**: Zhe Feng (zhe.feng@pnnl.gov)

#### Sketch of initial activities
- Follows MCSMIP protocol under [Tracking criteria](https://mcsmip.github.io/design/)
- Example notebook reading/remapping HEALPix data (link TBD)
- Standardize tracking output formats ([unify MCS mask files](https://github.com/WACCEM/MCSMIP-DYAMOND/blob/main/src/unify_mask_files.py))
- Example MCS mask files ([Globus link](https://app.globus.org/file-manager?destination_id=87909b37-fbcf-4735-a72e-1a406301a053&destination_path=%2Fsample_mcs_mask%2F&two_pane=true))
- Data sharing (upload instructions TBD)

---

### Shallow circulations in the ITCZ ([hk25-ShallowCirc](https://github.com/digital-earths-global-hackathon/hk25-teams/tree/main/hk25-ShallowCirc))

The intertropical convergence zone (ITCZ) in the eastern parts of the Pacific and Atlantic basins is dominated by bottom-heavy or shallow meridional circulations, with outflow observed at 2-4 km. In this team, we would like to understand the dynamical drivers of shallow meridional circulations as a function of the seasonal cycle using storm resolving simulations. We are interested in characterising the surface and free troposphere controls on the depth of the shallow circulations and testing the hypothesis that the circulation becomes more pronounced as the ITCZ moves poleward.

**Coordination**: Divya Sri Praturi (divya-sri.praturi@mpimet.mpg.de) and Marius Winkler (marius.winkler@mpimet.mpg.de)

#### Sketch of initial activities
* construct the meridional overturning circulation in the eastern Atlantic and Pacific ITCZ
* compute zonal and meridional momentum budgets across pressure levels
* determine the seasonal cycle of the depth of the outflow

---

### Mesoscale structure of stratocumulus ([hk25-StCu](https://github.com/digital-earths-global-hackathon/hk25-teams/tree/main/hk25-StCu))

Low-level clouds over subtropical oceans are important for the energy balance of the planet and climate sensitivity. Their properties and evolution crucially depend on small scale processes. A recent examination of their climatology ([Nowak et al. 2025](https://doi.org/10.1029/2024MS004340)) in two [NextGEMS](https://nextgems-h2020.eu/) global storm-resolving models indicated realistic covariability of stratocumulus and related environmental factors, and the vertical structure of the boundary layer. How is that possible without elaborated model tuning and on the grid which is too large to resolve large turbulent eddies?

It was speculated that the km-scale grid allows to simulate mesoscale circulations which might be sufficient to crudely represent the radiation-turbulence-entrainment-flux feedback regulating the behavior of stratocumuli. We would like to test this hypothesis by inspecting the mesoscale patterns of cloudiness, circulation and precipitation in the models and check whether those patterns comply with the mechanisms proposed to explain the cellular cloud structures evident in observations (see e.g. [Comstock et al. 2005](https://doi.org/10.1175/JAS3567.1), [van Zanten and Stevens 2005](https://doi.org/10.1175/JAS3611.1), [Wood et al. 2011](https://doi.org/10.5194/acp-11-2341-2011)).

**Coordination**: Jakub Nowak (jakub.nowak@mpimet.mpg.de)

#### Sketch of initial activities
* Extract snapshots of subtropical stratocumulus fields
* Asses qualitatively whether the mesoscale cloud patterns are cellular
* Quantify their organization with a chosen statistical metric
* Examine the co-variability of clouds, circulation and precipitation

---

### Global representation of local extremes ([hk25-LocExt](https://github.com/digital-earths-global-hackathon/hk25-teams/tree/main/hk25-LocExt))

Climate extremes can develop on a wide range of spatial scales from continental to local. Global km-scale models allow us a global view on such extremes with local detail important for impacts for the first time. Here, we will use them to quantify the spatial variability lost at coarser resolutions typical for established global models (e.g. from CMIP6 or HighResMIP). This will allow us to identify regions where output resolution matters for the representation of extremes and build understanding of the underlying processes. Comparing different km-scale models will enable us to analyse cases where models agree or diverge and trace them back to model differences, for example in the treatment of deep convection.

In this team we will test what the added value of high-resolution output is for the spatial representation of climate extremes. We also aim to understand potential differences between models.

**Coordination**: Lukas Brunner (lukas.brunner@uni-hamburg.de)

#### Sketch of initial activities
* Calculate extreme indices (e.g., [ETCCDI](https://etccdi.pacificclimate.org/list_27_indices.shtml)) at the highest available resolution from all available models
* Analyze what and where spatial variability is lost at coarser resolutions
* Compare different extreme indices and models and understand disagreements

---

### Tropical Cyclones ([hk25-TropCyc](https://github.com/digital-earths-global-hackathon/hk25-teams/tree/main/hk25-TropCyc))

Tropical Cyclones (TCs) are intense organised convective systems that are responsible for nearly half of the worldwide disaster-related costs (CRED & UNDRR, 2020). Historically, they have been difficult to represent in coarse-resolution climate models because of their small size and their sensitivity to convective parametrisations. It has been shown that increasing resolution to 25km allows models to represent the number and distribution of cyclones correctly (Roberts et al. [2020](https://link.springer.com/article/10.1007/s00382-024-07138-w)), but the intensity remains largely underestimated, and the structure is not well represented (Bourdin et al. [2024](https://link.springer.com/article/10.1007/s00382-024-07138-w)). Baker et al. ([2024](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2024GL109841)) showed that increasing resolution up to 5km improves the intensity, the lifecycle and the structure of TCs in NextGEMS simulations.

In this team, we will investigate how TCs are represented in the new sets of simulations in terms of statistics, structure, lifecycle and link with the environment.

**Coordination**: Stella Bourdin (stella.bourdin@physics.ox.ac.uk), Masaki Satoh (satoh@aori.u-tokyo.ac.jp)

#### Sketch of initial activities:
  + Assess TCs statistics (e.g., intensity and intensification rates) using TempstExtremes
  + Assess tropical cyclones structure from snapshots
  + Assess environmental controls on TCs, e.g., moisture, potential intensity

---

### How realistic are GSRM clouds? ([hk25-CloudClimato](https://github.com/digital-earths-global-hackathon/hk25-teams/tree/main/hk25-CloudClimato))


This science team will compare GSRM cloud characteristics with diverse climatological observations (in situ, satellite, etc.) to assess the realism of different cloud types in the control climate of various models and identify potential mean state biases. The goal is to publish these analyses in an overview paper that can be used as a a reference for process papers dedicated to more specific analyses of shallow clouds, deep clouds, storm tracks, polar clouds, etc. The hackathon will be used as a kickstarter for this project and hopefully the collaboration will continue afterwards to try and submit the paper rapidly.

Coordination : Emilie Fons (emilie.fons@lmd.ipsl.fr)

#### Sketch of initial activities:
- standardize cloud characteristics that are available in all GSR models. Which models have outputs from a satellite simulator ?
- gather observational data for comparison (e.g., reanalysis, CERES, Earthcare, CMIP, etc.)
- plots : maps, latitudinal profiles, altitude profiles, cloud regime profiles, interranual/seasonal/diurnal variability

---

### Air-sea interaction in the tropics ([hk25-ASintTrops](https://github.com/digital-earths-global-hackathon/hk25-teams/tree/main/hk25-ASintTrops))

This activity is motivated by several open questions on how the tropical boundary layer and moist convection interact with the underlying ocean on scales 2 km - 200 km. For instance, how does the tropical atmosphere respond to SST heterogeneity at those scales? What sets air-sea interaction at low versus high wind speeds, or how do precipitation or cloudiness impact air-sea fluxes and the ocean mixed-layer?

In this team we want to analyze relationships between SST, air-sea fluxes, tropical convection and the ocean mixed at (sub)mesoscales, using those participating models that run a coupled ocean-atmosphere simulation.

Coordination: Louise Nuijens (Louise.Nuijens@tudelft.nl)

#### Sketch of initial activities:
* Analyze air-sea heat fluxes and wind stress as a function of SST, stability and wind speed
* Derive divergence and curl of wind speed and stress across SST gradients
* Derive coupling coefficients to evaluate the atmospheric feedback on wind (stress)
* Analyze mixed-layer depth as a function of air-sea fluxes and wind speed
* Composite air-sea fluxes as a function of cloud cover, radiation and precipitation

---

### Land-Atmosphere Interaction ([hk25-Land](https://github.com/digital-earths-global-hackathon/hk25-teams/tree/main/hk25-Land))

The land-atmosphere interaction is one of the key drivers of Earth's surface water and energy budgets. Among these, soil moisture plays a crucial role by regulating surface heat fluxes, which in turn influence boundary layer development and precipitation. These processes are fundamental to understanding convection, climate feedbacks, and extreme events such as droughts, heatwaves, and floods.
Unlike coarse-resolution global circulation models or regional km-scale models, global km-scale models can explicitly resolve convection and eliminate the need for prescribed large-scale circulation. This enables a more holistic and physically consistent representation of land-atmosphere processes.

In this team, we aim to identify global hotspots of land-atmosphere coupling and evaluate the added value of high-resolution global simulations in capturing the influence of soil moisture on extreme events. Specifically, we will assess how changes in soil moisture affect precipitation, heatwaves, and droughts through their impacts on surface heat fluxes and boundary layer dynamics.

**Coordination**: Ching-Hung Shih (f11229004@ntu.edu.tw)

Sketch of initial activities:
+ Identify global hotspots of land-atmosphere coupling using km-scale model output
+ Quantify soil moisture-precipitation feedback across different regions
+ Analyze where and how spatial variability is introduced in km-scale models compared to coarser-resolution models
