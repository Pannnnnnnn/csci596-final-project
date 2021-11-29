# Parallel FDTD Electromagnetic computation for Plasmonic Nanostructure

## _Abstract_

Plasmonic Nanostructure has attracted great scientific interests. For example, plasmonic nanostructures with nano-gaps concentrate light to a small volume, which can lead to many potential applications. While it is theoretically predicted that the optimal plasmonic hot spot is a gap of less than 1 nanometer between two metallic particles<sup>[1]</sup>. The field strength at the hot spot is very large but it is hard to measure the real field strength experimentally. Therefore, a high precision simulation is required to study the field distribution of electromagnetic wave inside the nanostructure and predict the field enhancement of the hot spot. Finite-difference time-domain (FDTD) is a numerical computation technique for constructing the electromagnetic field inside the structure. It belongs in the general class of grid-based differential numerical modeling methods (finite difference methods). The time-dependent Maxwell's equations (in partial differential form) are discretized using central-difference approximations to the space and time partial derivatives<sup>[2]</sup>. The total FDTD computing time is highly dependent on the grid size, in this case the computation efficiency becomes an issue when the grid size is less then 1nm. 

<p align="center">
<img src="https://github.com/Pannnnnnnn/csci596-final-project/blob/main/Picture1.png">
</p>
<p align="center">
<b>Figure 1. Overview of the inverse design process.<sup>[1]</sup></b><br>
</p>

In this proposal, parallel computing method will be applied to improve the precision and efficiency of a FDTD Electromagnetic simulation for plasmonic nanostructure. By decompose the whole computation region into multiple subcells, the original simulation can be divided into several sub-problems. All sub-problems can be then solved simultaneously using the parallel computing. Therefore, each sub-problem can have enough computation resources to study more detials in a smaller grid cell compared with the grid cell in original FDTD simulation. 

Not only the plasmonic nanostructure simulation, other electromagnetic simulation problems that requires extremely small grid size can also be realized with the assistance of parallel computing. More details and evidence would be discovered after applying a smaller grid size to explore the science and mechanism. Moreover, a larger scale simulation problem can also use the parallel computation to increase the computing efficiency. 

## _Specific Objectives:_
1. A FDTD simulation script written in Java.
2. The grid decomposition of above simulation problem, a reasonable grid size of each subcell shoule be consider.
3. Comparison of the final simulation results with different grid sizes to find out how the grid sizes affect the simulation.
   
## _Task List:_
  - [x] A FDTD simulation script written in Java.
  - [ ] What grid size of each subcell shoule be considered?
  - [ ] Effect of different grid sizes on final simulation result.

## _Reference:_
[ [1] Song, B., Yao, Y., Groenewald, R. E., Wang, Y., Liu, H., Wang, Y., ... & Wu, W. (2017). Probing gap plasmons down to subnanometer scales using collapsible nanofingers. ACS nano, 11(6), 5836-5843.](https://pubs.acs.org/doi/abs/10.1021/acsnano.7b01468?casa_token=eXaLPlht1-kAAAAA:FSKeIHI9pep0w7YBtLatMtJ-_StfX1_oTa8FuP1PxB-TyxneuH1SDTusQzVIBdC9jCqgN-1g8owrt9PM)

[ [2] Finite-difference time-domain method. (2021. November 11). In Wikipedia. https://en.wikipedia.org/wiki/Finite-difference_time-domain_method](https://en.wikipedia.org/wiki/Finite-difference_time-domain_method)

