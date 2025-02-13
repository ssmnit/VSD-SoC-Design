# VSD-SoC-Design
As part of the Workshop VSD SoC Design Course

# Open Source ASIC Design Implementation
For open-source ASIC design, we need open-source RTL designs, EDA tools, and PDK data. Initially, IC design and fabrication were done by a few companies like Intel. In 1979, Lynn Conway and Carver Mead separated design from fabrication, leading to "fabless" (design-only) and "pure-play fabs" (manufacturing-only) companies. The link between them became Process Design Kits (PDKs), which include design rules, libraries, and more. PDKs were restricted by NDAs, but in 2020, Google and SkyWater released the first open-source PDK for 130nm technology.
![image](https://github.com/user-attachments/assets/e94b1c5a-5e51-40b4-bb47-6633115abf76)

![image](https://github.com/user-attachments/assets/fec528c9-be35-436d-b448-82ea3c9e8e81)

![image](https://github.com/user-attachments/assets/4e76b484-d85c-4083-8d99-1b7bbd87b0f1)

![image](https://github.com/user-attachments/assets/8b928e35-29d7-4d3b-9ae9-a4b8f2446cdd)

Simplified RTL to GDSII Flow
![image](https://github.com/user-attachments/assets/8d48bd4f-00e8-46ae-a130-7322b6b64ea5)

OpenLAne SoC -
Main Goal of OpenLane ASIC Flow is to produce Clean GDSII (No LVC - Layout vs Schematic, DRC-Design Rule Checking, Timing Violation)

OpenLane is tuned for Skywater 130nm PDK
![image](https://github.com/user-attachments/assets/b3a11f7c-f1e3-4ca0-b048-b8e5b0a9e44b)
![image](https://github.com/user-attachments/assets/16010a59-1c92-4b62-8b66-46f60cbd5f9b)

OpenLane ASIC Flow
![image](https://github.com/user-attachments/assets/710580c7-4ba1-495d-8d2e-64b6654e902c)
![image](https://github.com/user-attachments/assets/ca91f45a-8b4c-4c45-a021-342fb412148a)

![image](https://github.com/user-attachments/assets/4f09af0e-c2ca-46ba-8453-7b88ae26ac0f)

![image](https://github.com/user-attachments/assets/fc2e40bd-5395-4154-bc20-c2becac84a87)

![image](https://github.com/user-attachments/assets/f4c210c8-23f3-48dd-823a-92e2615ebbb8)

![image](https://github.com/user-attachments/assets/89ce5bb9-933d-471e-8df8-c03259956cc5)

![image](https://github.com/user-attachments/assets/f2300c92-99ff-4219-9c7c-89031172f35c)

# Day 2 - Floorplanning
 We want to find out the dimensions of core and die of standard cells.
 ![image](https://github.com/user-attachments/assets/4792fd5a-fd93-4ebe-a8cf-5f128a93e556)    ![image](https://github.com/user-attachments/assets/9420efd4-27a9-420f-8d4e-5b886f6a1e1e)

Cell occupies 100% of the core area. So utilization factor is 100%.
Utilization factor = (Area occupied by netlist) / (Total area of the core)
Practically we go for 50-60% utilization factor.

Example - Aspect Ratio (or utilization factor) = 0.5
![image](https://github.com/user-attachments/assets/71b73682-95f4-41b6-8d41-abc927fefb05)

![image](https://github.com/user-attachments/assets/c25f1fdf-4a88-4bd7-9888-0860260791da)
Concept of pre-placed cells
![image](https://github.com/user-attachments/assets/da17e9a8-17c0-416b-a081-9113794f327b)
![image](https://github.com/user-attachments/assets/439421a0-cc4a-4c2a-8ff1-b6fbbe30ac49)

De-coupling Capacitors
![image|250](https://github.com/user-attachments/assets/dc9c71e5-493b-4cdf-90d7-8fc7611d985e )
![image|250](https://github.com/user-attachments/assets/377cb8e4-490d-4025-b6bc-55e856c73cb4 )

Power Planning
All the elements of the circuit demanding current at the same time and decoupling capacitor is supposed to provides charge to all the elements. Sometimes it is not possible that all the macro would be connected to decoupling capacitor from the direct supply.
![image](https://github.com/user-attachments/assets/23cff40c-6fc9-4c51-a249-fa2b447e4d84)
![image](https://github.com/user-attachments/assets/867da02f-9db2-4e1b-8840-69e28c51d95e)

To avoid voltage droop multiple points (or supply) are provided
![image](https://github.com/user-attachments/assets/cbf7dd47-d09b-448d-8310-61989d2d39f1)
![image](https://github.com/user-attachments/assets/85dc4c45-bbbd-4f58-8720-5cba35096820)

Pin placement and logical cell placement blockage
![image](https://github.com/user-attachments/assets/853bc000-cc46-4dd1-8cab-ae18e4dde263)

Complete Design 
![image](https://github.com/user-attachments/assets/56206c24-70ff-4b9b-aea8-8814a95e4c88)
![image](https://github.com/user-attachments/assets/ad3004fd-552e-4793-a996-25e5bf17711d)

clock ports are bigger in size than the i/o ports. Clock drives all the bocks of the chips so we need least resistance path to the signal to flow. Logical cell placement blockage to avoid making any cell in the area, the place is not used for placement of blocks.
![image](https://github.com/user-attachments/assets/320ae891-f922-4740-9501-53bc29b23831)














 








