
# Advanced Semiconductor Packaging

In this repository, we will look into the introduction of semiconductor packaging including various types based on applications. We will also explore the fabrication and manufacturing processes of these types, as well as reliability testing on the packages. Furthermore, we will simulate packaging and testing utilizing Ansys Electronics Tools. 


## Day 1: Introduction to Semiconductor Packaging 

The fabrication of semiconductors occurs in a Foundry, a large-scale facility equipped with advanced technology and maintained in clean rooms of classes 5, 7, 10, and 10,000 with controlled environments. These Foundries are typically maintained by companies such as Intel, TSMC, Samsung, and Integrated Device Manufacturers (IDMs) like Micron and SK Hynix. These Foundries utilize 12-inch silicon wafers that are diced and packaged for distribution to various suppliers.

The primary purpose of packaging is to prepare a bare silicon wafer for practical applications, serving two main functions: protecting semiconductor devices on a die and connecting dies to other dies.


Functionality (Wafer - Die) -> Personality (After Packaging)

```
Insert Image 
```
### How to choose the right package for the application 
The initial layer, known as the system board, comprises a printed circuit board (PCB) that serves as a connector for various components and circuits, facilitating the assembly of the entire system. Subsequently, a carrier layer is employed to accommodate the silicon die.
```
Insert Image 
```
### Packaging Connections and different types 
The first or bottom layer is a system board with Printed Circuit Board (PCB) which connects to other parts or circuits to build an entire system. Next, there is another layer called carrier on which silicon die is placed. 

#### Types of Carriers

->   Leadframe, laminate. plastic, ceramic, organic RDL (redistribution layer), Silicon, Glass.  

#### Difference vs Substrate and Interposer 

Substrate: It is like a foundation where all the electrical and mechanical connections are made for ICs 

Interposer: Intermediate layer often made with silicon/organic materials that facilitates connections between chips using TSV (Through Silicon Vias) and TLVs (Through Laminate Vias).

There are different package technology and they are listed the figure below.
```
Insert Images()
```

## Anatomy of Packages

There are three main packaging concepts 

#### Leadframe Packages

a) DIP (Dual In-line Package): Through-hole package with pins extending from the sides for PCB insertion.

b) QFN (Quad Flat No-lead): Surface-mount package with leads under the package for compact size and thermal performance.

c) Leadframe-CSP (Chip Scale Package): Compact chip-scale package using a leadframe and wire bonding.

d) Leadframe-QFP (: Gull-wing surface-mount package with leads on all four sides.

#### Laminate Packages

a) Wire bond PBGA (Plastic Ball Grid Arrays): Die connected to package substrate using gold wire bonds and mold compound.

b) Flip chip PBGA: Die is flipped and bonded directly to substrate using solder bumps and epoxy underfill.

c) PBGA: Plastic Ball Grid Array, a laminate-based surface-mount package with solder balls.

d) LGA: Land Grid Array with flat pads instead of solder balls, allowing socketed connections.

e) FC-CSP: Flip Chip Chip Scale Package combining flip-chip bonding and chip-scale size.

#### Advanced Package Substrates

a) 2D: Multiple dies placed side-by-side on a substrate.

b) 2.1D: 2D layout enhanced with a Redistribution Layer (RDL).

c) 2.3D: Dies mounted on an organic interposer for better routing.

d) 2.5D: Dies mounted on a silicon interposer for high-density interconnects.

e) 2.5D CoWoS (Latest - Chip on Wafer on Substrate): SoC and HBM stacked on silicon interposer over a substrate for high bandwidth and integration.
```
Insert Images()
```
## Classification of Packaging Technology
```
Insert Images()
```
Difference between CSP and PBGA 
## Classification of Packaging Technology
```
Insert Images()
```


## Day - 2 Introduction to Semiconductor Packaging 
