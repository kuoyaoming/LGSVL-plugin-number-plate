# LGSVL Plug

![Screenshot](https://github.com/kuoyaoming/collision_video_generator/blob/master/image/Screenshot.png
)

# Introduction

This Plug can add the registration plate model on custom vehicle, it include two version.

v1 will random show one for five number plate (Taiwan format) and add it on the car model.
![v1]()
v2 will generate number plate from three random alphabet and three random number.
![v2]()
### list of custom vehicle：
* Jaguar: Jaguar2015XE modify from [https://github.com/lgsvl/Jaguar2015XE](https://github.com/lgsvl/Jaguar2015XE).
![Jaguar]()
* Police car: Taiwan style Police car.
![Police car]()
* Ambulance: Taiwan style Ambulance.
![Ambulance]()
* Fire Trunk: Taiwan style Fire Trunk.
![Fire Trunk]()

# Usage

1. Follow the [Build instructions](https://www.lgsvlsimulator.com/docs/build-instructions/) of LGSVL, cheak you can build Simulator from source.
2. Copy the script to the smae folder and replace it.
```
git clone https://github.com/kuoyaoming/collision_video_generator
cp .LGSVL-plug\v1\Script\ \(name\of\Simulator\distro)\
```
3. Build Simulator.
4. Copy the vehical model to build export diratry.
```
cp .LGSVL-plug\v1\Models\ \(name\of\build\distro)\
```
4. Open Simulator that you build, add new vehicl \(name\of\build\distro)\AssetBundles\Vehicles\(Vehicle\name).
5. Copy vehicles_config.json to vehicl Configuration .
6. Run Simulator
