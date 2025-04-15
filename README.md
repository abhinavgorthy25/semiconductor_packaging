
# Advanced Semiconductor Packaging

In this repository, we will look into the introduction of semiconductor packaging including various types based on applications. We will also explore the fabrication and manufacturing processes of these types, as well as reliability testing on the packages. Furthermore, we will simulate packaging and testing utilizing Ansys Electronics Tools. 


## Day 1: Introduction to Semiconductor Packaging 

The fabrication of semiconductors occurs in a Foundry, a large-scale facility equipped with advanced technology and maintained in clean rooms of classes 5, 7, 10, and 10,000 with controlled environments. These Foundries are typically maintained by companies such as Intel, TSMC, Samsung, and Integrated Device Manufacturers (IDMs) like Micron and SK Hynix. These Foundries utilize 12-inch silicon wafers that are diced and packaged for distribution to various suppliers.

The primary purpose of packaging is to prepare a bare silicon wafer for practical applications, serving two main functions: protecting semiconductor devices on a die and connecting dies to other dies.


Functionality (Wafer - Die) -> Personality (After Packaging)

![image](https://github.com/user-attachments/assets/4d447997-8ff4-4cc1-9381-ad81251a905c)

### How to choose the right package for the application 
The initial layer, known as the system board, comprises a printed circuit board (PCB) that serves as a connector for various components and circuits, facilitating the assembly of the entire system. Subsequently, a carrier layer is employed to accommodate the silicon die.
![image](https://github.com/user-attachments/assets/7be674ee-eb9e-4556-a51d-52fcc71d372b)

### Packaging Connections and different types 
The first or bottom layer is a system board with a Printed Circuit Board (PCB) which connects to other parts or circuits to build an entire system. Next, there is another layer called a carrier on which the silicon die is placed. 

#### Types of Carriers

->   Leadframe, laminate. plastic, ceramic, organic RDL (redistribution layer), Silicon, Glass.  

#### Difference vs Substrate and Interposer 

Substrate: It is like a foundation where all the electrical and mechanical connections are made for ICs 

Interposer: Intermediate layer often made with silicon/organic materials that facilitates connections between chips using TSV (Through Silicon Vias) and TLVs (Through Laminate Vias).

There are different package technologies, and they are listed in  the figure below.

![image](https://github.com/user-attachments/assets/28994f76-66ed-493b-92d4-04c25a2ffd8d)
![image](https://github.com/user-attachments/assets/c6ac3972-c3d4-4c2c-9c5d-f9dcdfe32628)


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

![image](https://github.com/user-attachments/assets/1c11f517-c524-4e05-8271-26dd7338a94e)

## Classification of Packaging Technology
![image](https://github.com/user-attachments/assets/f3ee4292-b625-4ed0-ab9a-df21f503fc5f)
![image](https://github.com/user-attachments/assets/85683b0a-362d-4625-a3d2-d72f3d169dca)




## Day - 2 Introduction to Semiconductor Packaging 

### Package Manufacturing - Review of Supply Chain 

![image](https://github.com/user-attachments/assets/12e1fad7-a39d-4fb1-bc8d-14b86446f959)
![image](https://github.com/user-attachments/assets/0380825f-76e0-4fed-a7eb-3812f9617bc7)


Key Abbreviations 

ATMP - Assembly, Testing, Marking and Packaging

OSAT - Outsourced Semiconductor Assembly and Test 

## Wafer Preparation and Dicing Process

| Step | Process                                           | Purpose                                                                                   | Importance                                                                                          |
|------|---------------------------------------------------|-------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| 1    | **Wafer Preparation Area (ISO Class 7)**          | This cleanroom environment ensures a low level of airborne particles (Class 7 = <10,000 particles/ft³). | Prevents contamination during wafer handling and processing.                                       |
| 2    | **Incoming Wafer Carrier**                        | A cassette or FOUP (Front Opening Unified Pod) holds multiple silicon wafers.             | Used to safely transport and store wafers before processing.                                        |
| 3    | **Wafer Inspection**                              | Optical or automated inspection tools scan the wafer.                                     | Detect surface defects, contamination, and pattern misalignments before further processing.         |
| 4    | **Wafer Front Tape Lamination**                   | Protective tape is laminated onto the top (front) surface of the wafer.                   | Protects circuits from contamination and physical damage. Holds diced die in place after the wafer is cut. |
| 5    | **Wafer Backside Grinding**                       | The backside of the wafer is thinned using a grinding wheel.                              | Reduces wafer thickness for improved thermal and electrical performance. Prepares the wafer for packaging. |
| 6    | **Tape Frame Mounting to Wafer Backside**         | Wafer is mounted onto a tape frame (a ring with adhesive film).                           | Holds wafer in place during dicing. Ensures stability and alignment for laser and blade tools.      |
| 7    | **Two-Step Wafer Dicing (Laser Grooving + Blade Dicing)** | **Step 1 – Laser Grooving:** Laser weakens streets (spaces between dies). **Step 2 – Blade Dicing:** Diamond blade cuts through the wafer. | Reduces stress and improves accuracy during blade dicing. Precision is critical to avoid chipping and damage.

![image](https://github.com/user-attachments/assets/9193da7b-6955-4de7-9f39-87011a6c50fe)

### Wire Bonding Packaging Flow 

![image](https://github.com/user-attachments/assets/d40268b5-b323-4ffd-b257-db10bc269950)


### Flip-Chip Packaging Flow

![image](https://github.com/user-attachments/assets/b69c0e8f-48fd-432d-b53f-8fc36d40c1c5)

### Wafer - Level Packaging (Fan out Wafer Level Packaging) - Advanced Packaging 

As semiconductor devices advance (especially in high-end processors, SoCs, and AI chips), the interconnect density increases — meaning more I/Os need to be routed in a very small area. This causes challenges in traditional packaging due to:

 1) Limited space for routing signals out of the die (called fan-out).

    2) Signal integrity and power delivery issues.

    3) Mechanical stress on solder bumps due to high pin counts.

![image](https://github.com/user-attachments/assets/985da015-0387-49ed-a9b1-c466f679b456)

### Why Fanout? 

1) Fan-out refers to the ability to spread out the connections (I/Os) from the chip (die) to a larger area.

2) Fan out Wafer Level Packaging does this by embedding the die in a molded material and adding Redistribution Layers (RDL) around the die.

3) These RDLs are metal interconnect layers (like BEOL in ICs), which reroute the signals from the tiny pads on the die to larger and more accessible solder balls.


## Day - 4 Package Testing 

![image](https://github.com/user-attachments/assets/78dab5e5-5ddb-46a1-86ec-889ca975b286)
![image](https://github.com/user-attachments/assets/6be89da3-610b-4e3d-bcd5-8abe2f4df22c)
![image](https://github.com/user-attachments/assets/6f3e7316-2cd7-494a-95a1-b9034866f163)


### Bathtub Curve Phases

| Phase                  | Description                                                                 | Curve Shape       | Failure Causes                                      | Burn-in Relevance                          |
|------------------------|-----------------------------------------------------------------------------|-------------------|-----------------------------------------------------|--------------------------------------------|
| Infant Mortality     | High initial failure rate due to manufacturing defects or weak components. | Decreasing        | Dielectric breakdown, metallization issues, etc.   | **Target phase** – Burn-in removes weak parts |
| Useful Life          | Low, steady failure rate; components perform reliably.                     | Flat              | Random external factors, minor process variations   | Burn-in-tested components operate here     |
| Wear -out            | Failure rate increases as devices age and degrade.                         | Increasing        | Electromigration, oxide wear-out, thermal fatigue   | Not addressed by burn-in                   |

![image](https://github.com/user-attachments/assets/2c4b5b73-ea58-41d6-976d-b7ccce002cd9)
![image](https://github.com/user-attachments/assets/39e9244e-e677-4544-b096-13bf26822902)
![image](https://github.com/user-attachments/assets/17427585-b6cd-45b7-9d21-6f3118fa2ad9)




