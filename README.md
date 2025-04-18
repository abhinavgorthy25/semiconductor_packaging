
# Advanced Semiconductor Packaging

In this repository, we will look into the introduction of semiconductor packaging including various types based on applications. We will also explore the fabrication and manufacturing processes of these types, as well as reliability testing on the packages. Furthermore, we will simulate packaging and testing utilizing Ansys Electronics Tools. 


## Day 1: Packaging Evolution: From Basics to 3D Integration

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




## Day - 2 From Wafer to Package: Assembly and Manufacturing Essentials 

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
| 2    | **Incoming Wafer Carrier**                        | A cassette or FOUP (Front Opening Unified Pod) holds multiple silicon wafers.             | Used to transport and store wafers before processing safely.                                        |
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


### Day - 3 Thermal Simulation of Semiconductor Packages with ANSYS.

### Getting Started with ANSYS Electronics Desktop 

Use this link to Download ANSYS Electronics Desktop:
```
https://www.ansys.com/academic/students/ansys-electronics-desktop-student

```
Select the desired package: Go to IcePak -> ToolKit -> Geometry -> Packages -> Select the desrired package 
![Screenshot 2025-04-16 at 5 20 59 PM](https://github.com/user-attachments/assets/15c9cf4e-24fd-4d47-94e4-28af63bc8d17)

### Properties of Flip Chip Ball Grid Arrays: 

![Screenshot 2025-04-16 at 5 23 41 PM](https://github.com/user-attachments/assets/cc90c14f-dd1d-441d-baca-6d51937d207e)

 ### 3D Model of Flip Chip BGA: 
![Screenshot 2025-04-16 at 5 34 38 PM](https://github.com/user-attachments/assets/75f624ae-63ac-435d-b12c-ec9712561f61)

### Thermal Model:  
The boundary conditions are set to view a proper thermal analysis. In the thermal model, the total power is set to 1 W. 

![Screenshot 2025-04-16 at 5 39 45 PM](https://github.com/user-attachments/assets/a0979508-01a8-476c-8a7d-1862944d2f82)
![Screenshot 2025-04-16 at 5 42 40 PM](https://github.com/user-attachments/assets/4f9081b6-fabf-441b-8a8b-6361a2b372e2)
In the source, Ambient temperature is selected: 
![Screenshot 2025-04-16 at 5 43 36 PM](https://github.com/user-attachments/assets/67f34d8a-b38c-4f5b-af09-386348602cc3)
### Monitor: 
To view the analysis, a point monitor is selected for all the layers and temperature is selected for all. 

![Screenshot 2025-04-16 at 5 45 27 PM](https://github.com/user-attachments/assets/58fea2ec-c44a-47cb-8c4b-fe033b18ef1d)
![Screenshot 2025-04-16 at 5 46 04 PM](https://github.com/user-attachments/assets/b62b3171-ad1a-4734-a1a3-f0c1ddf60c1c)

Make sure every simulation mentioned in the right column is completed and move on to the meshing by clicking on “Meshing” and “Generate Mesh”. Now, a mesh is generated. 

![Screenshot 2025-04-16 at 5 49 08 PM](https://github.com/user-attachments/assets/bf42c290-ec82-482d-aaa5-581f949a472a)

Now, in Analysis , right click on it to find Solve Setup and click OK 
![Screenshot 2025-04-16 at 5 56 00 PM](https://github.com/user-attachments/assets/7531199a-03c5-4aa2-8946-2995b22802d6)

### Validation: 
Locate the “Validate” button at the top of the screen and ensure that each layer of analysis is marked as “checked.” 
![Screenshot 2025-04-16 at 5 56 29 PM](https://github.com/user-attachments/assets/1b347701-4242-4f6a-b7d3-947d0d8a46cf)
![Screenshot 2025-04-16 at 7 00 43 PM](https://github.com/user-attachments/assets/6c9e0ba3-f29c-44e3-8e12-59e3b9563e7a)

Merge the meshing for underfill: Click on Solids -> Underfill and click on Merge Meshing and click on Analyse all to ensure overall meshing. 

After successful meshing, try to select the desired area and select plot fields and temperature to see the temperature plots. 

<img width="1000" alt="Screenshot 2025-04-17 at 11 34 23 AM" src="https://github.com/user-attachments/assets/f5270f56-26df-4652-90f5-ce69fd596623" />

Enable Specify Name, Specify Folder, Plot on Surface only and click "DONE"
<img width="1000" alt="Screenshot 2025-04-17 at 11 35 36 AM" src="https://github.com/user-attachments/assets/2c711897-d19a-4205-a9be-ce260e0d7648" />

Now, you will see the thermal response of the entire FCGBA package: 
<img width="1000" alt="Screenshot 2025-04-17 at 11 37 14 AM" src="https://github.com/user-attachments/assets/62413682-0623-452a-9b23-1af59358f4f3" />

By employing IcePak tools from ANSYS Desktop, we can conduct a comprehensive thermal simulation analysis. You can also select different packages and perform the basic thermal simulation. 


## Day - 4 Ensuring Package Reliability: Testing and Performance Validation

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

## Day - 5 Lab - 2 Creating the semiconductor package cross-section in Ansys AEDT

<img width="1000" alt="Screenshot 2025-04-17 at 12 01 13 PM" src="https://github.com/user-attachments/assets/d6cf7ce4-f363-4ef8-87db-f6478b18d344" />

### Task 1: Creating a Die: 3 x 3mm , Thickness: 0.2mm 

![Screenshot 2025-04-17 at 3 47 26 PM](https://github.com/user-attachments/assets/500084ca-bb94-4cb7-9c78-d2164fff1350)

Thicken the sheet by selecting Rectangle and click on Modeler -> Surface -> Thicken sheet -> Desired Thickness (Here it is 0.2 mm) 

![Screenshot 2025-04-17 at 3 47 42 PM](https://github.com/user-attachments/assets/c0de63dd-460d-419d-a807-a158a8958c66)

### Task 2:  Creating a Substrate, 
Construct a second rectangle  (Area: 3 x 3mm, Thickness: 0.2mm) for the substrate and rename the previous one to “Die.” and the present one to "Substrate" .Subsequently, modify the material properties to Silicon for "Die". 

![Screenshot 2025-04-17 at 5 21 12 PM](https://github.com/user-attachments/assets/e665a446-2d6a-4fbb-8b3d-7df2910ceb1b)
Change the substrate material to Epoxy: 

![Screenshot 2025-04-17 at 5 42 07 PM](https://github.com/user-attachments/assets/63a9e7ab-0b38-49e1-86f1-b5758338e5f1)
### Task 3: Creating Die Attach and Bond pads:

Similarly, construct the Die attach and bond pads by definition dimensions and materials. 

![Screenshot 2025-04-17 at 5 48 08 PM](https://github.com/user-attachments/assets/90b6ca7c-923c-4919-931d-f50ab2bd2c2f)
![Screenshot 2025-04-17 at 6 06 02 PM](https://github.com/user-attachments/assets/a8c0e8c1-aa09-44d6-8e57-86c175ec0a47)

### Task 4: Wirebonding 

Draw a wire bond and change its properties as required. (Here it is set to default) 

![Screenshot 2025-04-17 at 6 06 50 PM](https://github.com/user-attachments/assets/0f1a016b-e28c-4ab9-818e-1c939528cd7f)

In wire bonding, the metal must be ductile to ensure reliable connections. Consequently, gold is the most commonly used material in wire bonding. 

### Task 5: Encapsulating with Mold Compound. 

![Screenshot 2025-04-17 at 6 51 02 PM](https://github.com/user-attachments/assets/fc4c41ea-9c65-40fd-a686-c90ba8e7dcbf)

Laser marking is performed on the Mold component, necessitating adequate headroom to ensure the integrity of wirebonds. 

![Screenshot 2025-04-17 at 6 57 10 PM](https://github.com/user-attachments/assets/b4b39a2c-32ff-4b3f-aa4b-84cfc9822482)

The subsequent procedure involves attaching the solder balls to the substrate. This process elucidated the methodology for constructing a package and subsequently simulating its thermal behavior. 

## Acknowledgements

I extend my sincere gratitude to Mr. Kunal Ghosh for providing this opportunity and to the team at IIT Gandhinagar for sharing their expertise. 




