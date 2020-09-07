# Introduction
This Plug can add the registration plate model on a custom vehicle, it includes two versions.

v1 will randomly show one for five number plates (Taiwan format) and add it to the car model.
![v1](https://github.com/kuoyaoming/LGSVL-plugin-number-plate/blob/master/.image/v1.png)
v2 will generate a number plate from three random alphabets and three random numbers.
![v2]()
### list of custom vehicle：
* Jaguar: Jaguar2015XE modify from [https://github.com/lgsvl/Jaguar2015XE](https://github.com/lgsvl/Jaguar2015XE).
![Jaguar](https://github.com/kuoyaoming/LGSVL-plugin-number-plate/blob/master/.image/j.png)
* Police car: Taiwan style Police car.
![Police car](https://github.com/kuoyaoming/LGSVL-plugin-number-plate/blob/master/.image/p.png)
* Ambulance: Taiwan style Ambulance.
![Ambulance](https://github.com/kuoyaoming/LGSVL-plugin-number-plate/blob/master/.image/a.png)
* Fire Trunk: Taiwan style Fire Trunk.
![Fire Trunk](https://github.com/kuoyaoming/LGSVL-plugin-number-plate/blob/master/.image/f.png)

# Usage

1. Follow the [Build instructions](https://www.lgsvlsimulator.com/docs/build-instructions/) of LGSVL, cheak you can build Simulator from source.
2. Copy the script to the same folder and replace it.
```
git clone https://github.com/kuoyaoming/collision_video_generator
cp .LGSVL-plug\v1\Script\ \(name\of\Simulator\distro)\
```
3. Build Simulator.
4. Copy the vehicle model to directory from build export.
```
cp .LGSVL-plug\v1\Models\ \(name\of\build\distro)\
```
5. Open Simulator that you build, add new vehicle \(name\of\build\distro)\AssetBundles\Vehicles\(Vehicle\name).
6. Copy vehicles_config.json to vehicle configuration .
7. Run Simulator
