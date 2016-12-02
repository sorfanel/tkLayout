Pixel models

Baseline_tilted_200_Pixel_1_1_1.cfg  Square pixels everywhere (small L1-2 and R1-2)
Baseline_tilted_200_Pixel_1_1_2.cfg  Like 1.1.1, but without DC/DC converters 
Baseline_tilted_200_Pixel_1_2_1.cfg  Like 1.1.1, but Rectangular pixels in barrel
Baseline_tilted_200_Pixel_1_3_1.cfg  Like 1.1.1, but Rectangular everywhere
Baseline_tilted_200_Pixel_1_4_1.cfg  Like 1.3.1 But a bit shorter barrel
Baseline_tilted_200_Pixel_1_5_1.cfg  Like 1.3.1 But a lot shorter barrel
Baseline_tilted_200_Pixel_1_5_2.cfg  Like 1.5.1, but without DC/DC converters

Baseline_tilted_200_Pixel_3_5_1.cfg  2-rings step Like, TEDD and FPIX_2 disks moved to allow insertion -- small pixels everywhere

Baseline_tilted_200_Pixel_4_0_0.cfg  Like 3_5_1, but with 22x16.4 mm^2 chips (good for tilt?)
                                     BPIX=25x100 FPIX1=50x50 FPIX2=25x100

Baseline_tilted_200_Pixel_4_0_1.cfg  Like 4_0_0, but BPIX=50x50
                                     i.e. BPIX=50x50 FPIX1=50x50 FPIX2=25x100

Baseline_tilted_200_Pixel_4_0_2.cfg  Like 4_0_0, but FPIX1=25x100
                                     i.e. BPIX=25x100 FPIX1=25x100 FPIX2=25x100

Baseline_tilted_200_Pixel_4_0_3.cfg  Like 4_0_2, but
                                     FPIX2=50x50

Baseline_tilted_200_Pixel_4_0_2_1.cfg Like 4_0_2, but with 7 FPIX1 disks and 4 FPIX2 disks

OT_Tilted_360_200_Pixel_4021.cfg     First OT-numbered version: 3.6.0
                                     Pixel version 4.0.2.1
                                     Contains the new 2S barrel, with 3x multiplicity
                                     Contains new tilted barrel version 2016-07-15 (by kamil Cichy)

OT_Tilted_361_200_Pixel_4021.cfg     OT Version 3.6.1
                                     Pixel version 4.0.2.1
                                     Small adjustment in tilted barrel positions (version 2016-07-16 by Kamil Cichy)

OT_Tilted_362_200_Pixel_4021.cfg     OT Version 3.6.2
                                     Pixel version 4.0.2.1
                                     VERY small adjustment in positioning of TBPS layer 1 ring 8 and 10 (affexts rings 8+)

OT_Tilted_362_200_Pixel_4022.cfg     OT Version 3.6.2
                                     Pixel version 4.0.2.2 <- like 4.0.2.1 but with lower radii for BPIX L3 and L4 (less modules)

OT_Tilted_363_200_Pixel_4021.cfg     OT Version 3.6.3 !! Work in progress !!
                                     This is just an intermediary version towards an optimized TBPS. Main optimization point
                                     should be the reduction of TBPS planks δ and Δ, by 5 mm and 1 mm respectively
                                     Position of first ring (by changing zOverlap) was moved in such a way to keep the distance between the centre of the last flat module and the centre of the first
                                     tilted module (in z)
                          (3.6.2)    z_last_flat z_inner_first_tilted zOverlap zError_outer
                                     121.212     170.363              1.0      3.572 
                                     213.069     265.499              1.0      6.262
                                     305.080     355.757              1.5      13.725
                          (.....)    z_last_flat z_inner_first_tilted zOverlap zError_outer
                                     124.029     166.827              18       57.977
                                     216.018     262.683              16       89.562
                                     307.947     352.500              17       138.486

                                     Radii and zOverlap of first rings were then changed so as to obtain zError_outer ~50mm, ~70mm, ~70mm for layers 1, 2, 3 at the transition
                                     Layer  Radius [mm]        zOverlap [mm]  zError_outer
                                     1      227.5   -> 228.0   18 -> 16       57.977   -> 52.231
                                     2      355.175 -> 356.7   16 -> 12.5     89.562   -> 73.053
                                     3      508     -> 511     17 ->  8.5     138.486  -> 75.649

OT_Tilted_364_200_Pixel_4021.cfg     OT Version 3.6.4 !! Work in progress !!
                                     Starting the same process as for 3.6.3, with updated δ
                                     Layer 1: δ = 3.9mm
                                     Layer 2, 3: δ = 3.4mm
                                     Since the first tilted ring -> last flat ring had a Δz = 43.58 mm and was already considered to be "close"
                                     and the δ reduction caused this number to further shrink (down to 43.33) , we adjusted zOverlap (16.0 → 15.5)
                                     to push back Δz to 43.62 (basically the same as 3.6.3). Layer 2 and 3 are not expected to be troublesome with a
                                     Δz(last flat → first tilted) = 47.1 and 46.8 respectively).
                                     Overall the change 3.6.3 → 3.6.4 had a positive effect on the coverage of tracks from the origin, with
                                     zErrorOuter = { 51.8, 76.0, 78.8 }: a slight reduction for layer 1 and an increase for layers 2 and 3

                                     
OT_Tilted_462_200_Pixel_4021.cfg     OT Version 4.6.2 <- like 3.6.2 but Avi-style
                                     Pixel version 4.0.2.1


Baseline_tilted_200_Pixel_4_1_0.cfg  Like 4_0_0, but with tilted BPIX


OT_Tilted_362_200_Pixel_4023.cfg     OT Version 3.6.2
                                     Pixel version 4.0.2.3 <- like 4.0.2.1 but with 8 FPIX_1 disks and 4 FPIX_2 disks

OT365_200_IT4022.cfg                 OT Version 3.6.5  <- like 3.6.4 but with adjusted tilted ring positions and increased layer radii
                                     Inner tracker version 4.0.2.2

OT365_200_IT4024.cfg                 OT Version 3.6.5  <- like 3.6.4 but with adjusted tilted ring positions and increased layer radii 
                                     Inner tracker version 4.0.2.4 <- like 4.0.2.3 but with smaller barrel radii, just like 4.0.2.2 

OT365_200_IT4025.cfg                 OT Version 3.6.5
                                     Inner tracker version 4.0.2.5 <- based on 4.0.2.4 but with
                                     BPIX_4.3.0 adjusted radii: #rods reverted to 12,28,24,32
                                                                smaller overlap (0.6mm) in L2
                                                                bigger overlap (2.0mm) in L3,4
                                                                radii 29.000, 70.146, 117.753, 157.388
                                     and FPIX_2 shifted by 10 cm inwards
                                            disk z: 1750.0, 1985.43, 2250.83, 2550.0

