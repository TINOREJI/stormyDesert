# Stormy Desert with Sand Dunes

Let's embark on a mesmerizing journey into the heart of nature's tumultuous beauty with this captivating Blender project. As we delve into the arid expanse of a desert landscape entwined with the dramatic dance of a stormy sky, let the meticulous 3D modelling, dynamic lighting, and atmospheric effects transport you to a realm where tranquillity converges with chaos.

## Packages and Assets Downloading


```bash
Download the necessary materials required accordingly.
Materials:- sand[BlenderKit]
Assets   :- Animal Skull, Desert Grass/Cactus[BlenderKit/3D Modeling]
HDR's    :- Desert Sky/Evening Sky[BlenderKit/Polyhaven( https://polyhaven.com/ )]
```


## Desert Base Creation


Open Geometry Nodes and create Nodes as below with same values.

 ![33](https://github.com/TINOREJI/stormyDesert/assets/95184183/784d09e8-c017-4196-a162-9723ad717875)

 
 ##### Output:
  ![image](https://github.com/TINOREJI/stormyDesert/assets/95184183/a620767a-4bb3-4596-8f8a-6ebc100532c6)


## Desert Dune Shaping


 Open Geometry Nodes and create Nodes as below with same values.
 
 ![Screenshot 2024-02-11 042106](https://github.com/TINOREJI/stormyDesert/assets/95184183/811751e5-258a-470c-b444-cc9edd212aae)
 
 
 ##### Output:
  
 ![Screenshot 2024-02-11 042117](https://github.com/TINOREJI/stormyDesert/assets/95184183/fbe40eb0-7b03-4022-a8bc-4246fd8a8483)

## Desert Wave Structure Making and Adjusting


 Open Geometry Nodes and create Nodes as below with same values.
  ![Screenshot 2024-02-11 042629](https://github.com/TINOREJI/stormyDesert/assets/95184183/9c9895ea-4dba-4dbc-ab25-dedc390e8503)


 ##### Output:
  ![Screenshot 2024-02-11 042646](https://github.com/TINOREJI/stormyDesert/assets/95184183/1e40c271-0cb8-4adc-b8eb-2761edfea2de)


## Desert Design Adjusting.


 Open Geometry Nodes and create Nodes as below with same values.


  ![Screenshot 2024-02-11 044402](https://github.com/TINOREJI/stormyDesert/assets/95184183/763b89af-b871-428f-8f3c-c33de5e50859)

 ##### Output:
   ![Screenshot 2024-02-11 043703](https://github.com/TINOREJI/stormyDesert/assets/95184183/7fbafdf4-4435-4e7a-a37a-2d5eacfcc223)


## Desert Material Adding and Adjusting.


 Open Geometry Nodes and create Nodes as below with same values.

  ![image](https://github.com/TINOREJI/stormyDesert/assets/95184183/57e0ce80-9937-4412-9323-518b2c67a074)

 
 ##### Output:
  ![image](https://github.com/TINOREJI/stormyDesert/assets/95184183/b4a7dfa4-2ca7-4a11-b1bb-f47e7384784d)


## Desert Grass Adding and Adjusting.


 Open Geometry Nodes and create Nodes as below with same values.
  ![image](https://github.com/TINOREJI/stormyDesert/assets/95184183/283ea21a-c3e6-4ee9-9b73-e51812d35720)

 
 ##### Output:
  ![image](https://github.com/TINOREJI/stormyDesert/assets/95184183/21eb8e4a-a82a-481a-b1be-b4c68b85c793)


## Adding animal Skull


 Search for animal skull in BlendKit and drop it at a perfect position.
  ![image](https://github.com/TINOREJI/stormyDesert/assets/95184183/c5c3fc5f-3d78-46cf-a261-2be7ee1c9b21)


 
 ##### Output:
   ![image](https://github.com/TINOREJI/stormyDesert/assets/95184183/7314531f-3b66-4b7d-b779-5647a7fd1657)


## Creating Sand Storm Particle System.

 ### Create Sand Particle Using Sphere
  
  Using Proportional Editing create unique sand particles from sphere.
  ![Screenshot 2024-02-11 213549](https://github.com/TINOREJI/stormyDesert/assets/95184183/5a9a9fbb-7d2d-4457-b660-882fba1ac9bc)

  
  ##### Output:
   ![Screenshot 2024-02-11 213610](https://github.com/TINOREJI/stormyDesert/assets/95184183/4e0a2a53-b084-4175-90f0-11c7ba620b80)



 ### Create a particle system on a plane mesh added and adjust the fields according.
 #### Particle System
 ```bash
Particle Number  :  50000
Seed             :  67
Frame Start      : -60
End              :  500
Life Time        :  500
Normal           :  0
Rotation         :  Dynamic
Render as        :  Collection
Scale            :  0.002
Children         :  Simple
Render Amount    :  100
Seed             :  4
Radius           :  1
Roundness        :  0.5
Gravity          :  0.05
```

 ### Adding a Wind and Turbulance Force Fields with values:
  #### Wind
```bash
Force Field  : Wind
Wind Strength: 20
Flow         : 1
Seed         : 122
Wind Factor  : 1
```
  #### Turbulance
```bash
Force Field        : Turbulance
Turbulance Strength: 40
Size               : 8/10
Flow               : 0-1
Seed               : 38
```
 ### Adding a Smoke Emittor Using a Cube and Fast Animation with values:

 #### Smoke Emittor
  ```bash
  Fluid Type       : Domain
  Domain Type      : Gas
  Border Collision : Bottom
  Buoyancy         : -2
  Heat             : -2
  Dissolve         : Yes
  Time             : 80
  Slow             : Yes
  Frame Start      : 1
  End              : 250-400
```
## Output After Rendering:
##### Output:
   ![Uploading image.png…]()

 
