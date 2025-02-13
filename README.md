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


 








