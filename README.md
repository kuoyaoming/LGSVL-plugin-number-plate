# LGSVL Number Plate Plugin

Add registration plates to custom vehicles in the LGSVL/SVL Simulator. This repository includes two variants you can choose from.

## Versions

- v1: Randomly selects one of five Taiwan-style number plates and attaches it to the vehicle model.
  
  ![v1](https://github.com/kuoyaoming/LGSVL-plugin-number-plate/blob/master/.image/v1.png)

- v2: Generates a plate composed of three random letters followed by three random digits (e.g., ABC-123).

## Included custom vehicles

- Jaguar: `Jaguar2015XE`, modified from [https://github.com/lgsvl/Jaguar2015XE](https://github.com/lgsvl/Jaguar2015XE).
  
  ![Jaguar](https://github.com/kuoyaoming/LGSVL-plugin-number-plate/blob/master/.image/j.png)

- Police car: Taiwan style police car.
  
  ![Police car](https://github.com/kuoyaoming/LGSVL-plugin-number-plate/blob/master/.image/p.png)

- Ambulance: Taiwan style ambulance.
  
  ![Ambulance](https://github.com/kuoyaoming/LGSVL-plugin-number-plate/blob/master/.image/a.png)

- Fire truck: Taiwan style fire truck.
  
  ![Fire Truck](https://github.com/kuoyaoming/LGSVL-plugin-number-plate/blob/master/.image/f.png)

## Requirements

- A working local build of LGSVL/SVL Simulator from source. Follow the official guide: https://www.lgsvlsimulator.com/docs/build-instructions/

## Quick start

1) Clone this repository

```bash
git clone https://github.com/kuoyaoming/LGSVL-plugin-number-plate
cd LGSVL-plugin-number-plate
```

2) Choose a version (v1 or v2) and copy the script into your Simulator source tree

- Back up your original file first: `Assets/Scripts/Dynamics/Examples/VehicleSMI.cs`
- Then replace it with the version you want:

```bash
# Example for v1
cp -f v1/Script/Assets/Scripts/Dynamics/Examples/VehicleSMI.cs \<SIMULATOR_SOURCE_ROOT\>/Assets/Scripts/Dynamics/Examples/VehicleSMI.cs

# Example for v2
cp -f v2/Script/Assets/Scripts/Dynamics/Examples/VehicleSMI.cs \<SIMULATOR_SOURCE_ROOT\>/Assets/Scripts/Dynamics/Examples/VehicleSMI.cs
```

3) Build the Simulator from source (per the official guide)

4) Copy the provided vehicle AssetBundles into your built Simulator distribution

```bash
# v1 includes Jaguar example
cp -r v1/Models/AssetBundles/Vehicles/* \<SIMULATOR_BUILD_DIR\>/AssetBundles/Vehicles/

# v2 includes Police, Ambulance, Fire Truck
cp -r v2/Models/AssetBundles/Vehicles/* \<SIMULATOR_BUILD_DIR\>/AssetBundles/Vehicles/
```

5) Add vehicle configuration

Copy `vehicles_config.json` from the repository root into your Simulator's vehicle configuration location (or import via the Web UI if applicable). The exact directory may vary by build; a common setup is alongside other vehicle JSON files in the built distribution.

6) Run the Simulator and add the vehicles

- Open your built Simulator.
- Add a new vehicle by selecting the corresponding bundle under `AssetBundles/Vehicles/`.
- Ensure the vehicle configuration is recognized.

## Notes

- v1 uses a fixed set of Taiwan-style plates; v2 generates plates at runtime (three letters + three numbers).
- The provided assets are intended as examples. You can adapt the scripts to your own vehicles.

## Credits

- Jaguar asset based on `Jaguar2015XE`: https://github.com/lgsvl/Jaguar2015XE
