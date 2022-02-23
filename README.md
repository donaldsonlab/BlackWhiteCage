# BlackWhiteCage

This repository contains 3D models, created in Solidworks, and fabrication files for designing and constructing a Black and White Cage. This is divided into two
sections: one white with an open top and the other black and enclosed. The lid for the enclosed half integrates magnets for quick and quiet attachment and removal during 
experiments. For modularity, the rest of the cage is assembled using 3D printed brackets.

![alt text](/Images/BlackWhiteBox_openandclosed.jpg)

The walls of this chamber are laser cut out of clear 0.118" acrylic sheets and the floor is cut out of 0.22" acrylic for stability. They are then painted matte white and matte
black accordingly and assembled using 3D printed brackets. These brackets, along with the necessary fasteners, may be ommited if an adhesive
is used instead, making the assembly permanent. This is the method used for the [PPT](https://github.com/donaldsonlab/PPT-Chamber). The files used on the laser 
cutters are located in the [DXF](/DXF) directory. To optimize the nesting of parts on as few acrylic sheets as possible, we use an open source software called 
[Deepnest](https://deepnest.io/). The L-brackets, floor brackets, and magnet mounts are 3D printed on a Zortrax M200 Plus FDM printer with PLA, ABS, or Z-ULTRAT filament. The 
.STL files for printing are in the [STL](/STL) directory.

![[/Images/BlackWhiteBox_Assembly.jpg|width=100px]]


|       Bill of Materials      |
--------------------------------
|Item No.|Part|Description|Quantity|
-|----------------------|------------------------------------------------------------------------|-|
1|bw_floor             |Laser cut [bw_floor.dxf](/DXF/bw_floor.dxf)                                                         |1|
2|bw_sideWall          |Laser cut [bw_sideWall.dxf](/DXF/bw_sideWall.dxf)                                                   |2|
3|bw_frontBack         |Laser cut [bw_frontBack.dxf](/DXF/bw_frontBack.dxf)                                                 |2|
4|bw_doorway           |Laser cut [bw_doorway.dxf](/DXF/bw_doorway.dxf)                                                     |2|
5|bw_door              |Laser cut [bw_door.dxf](/DXF/bw_door.dxf)                                                           |1|
6|bw_lid               |Laser cut [bw_door.dxf](/DXF/bw_door.dxf)                                                           |1|
7|bw_magnetMount_Lid   |3D printed PLA/ABS [bw_magnetMount_Lid.stl](/STL/bw_magnetMount_Lid.stl)                            |2|
8|bw_magnetMount_Wall  |3D printed PLA/ABS [bw_magnetMount_Wall.stl](/STL/bw_magnetMount_Wall.stl)                          |2|
9|15x2mm Disk Magnets  |[Off-the-shelf 15x2mm refrigerator magnets](https://www.amazon.com/DIYMAG-Refrigerator-Magnets-Premium-Brushed/dp/B07G48647D) |4|
10|bw_LBracket         |Optional 3D printed PLA/ABS [bw_LBracket.stl](/STL/bw_LBracket.stl)                                 |4|
11|bw_floorBracket     |Optional 3D printed PLA/ABS [bw_floorBracket.stl](/STL/bw_floorBracket.stl)                         |4|
12|M3x8mm Screws       |Off-the-shelf screws required for magnet mounts but optional for brackets if using plastic cement   |16|
13|Plastic Cement      |Optional Plastruct Plastic Weld or IPS Weld-On 3 Acrylic Plastic Cement                             |<1|
14|Matte White Paint   |[Krylon Fusion All-In-One Spray Paint, Matte, White, 12 oz.](https://www.walmart.com/ip/Krylon-Fusion-All-In-One-Spray-Paint-Matte-White-12-oz/678882687)|<1|
15|Matte Black Paint   |[Black, Rust-Oleum American Accents 2X Ultra Cover Ultra Matte Spray Paint, 12 oz](https://www.walmart.com/ip/Black-Rust-Oleum-American-Accents-2X-Ultra-Cover-Ultra-Matte-Spray-Paint-12-oz/488512581)|<1|

The brand of acrylic cement is not important, as long as it can hold the acrylic pieces together. Similarly, the brand of paint is unimportant and can either be *matte* or 
*flat*, although matte finishes can typically withstand more cleaning. The magnets can also be sourced elsewhere, but the mounts are fitted for 15x2mm disk magnets.

**Note:** If the wall 
thickness is adjusted, the 3D models and .DXF files must also be modified. This can be done manually in the part files or by using the text file, 
[blackWhiteEquations.txt](blackWhiteEquations.txt), which contains equations used for each Solidworks part. Simply change the "WallThickness" and/or "FloorThickness" to the 
desired value and rebuild or refresh the part file.


