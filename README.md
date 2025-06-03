# Neptune 4 Pro – Z Axis Linear Rail Mounting System

This mod was inspired by the limitations and challenges imposed on Neptune printers by the TBStrong z rail kit.   Why do you need z rails at all?   Well, you don't, but I have them, and I never have to worry about aligning pom wheels, or any kind of z banding.   If you are here, you are interested in putting rails on the z axis, becuase you have probably already put the y axis rails and perhaps the x axis upgrade <link here for that git repo address>.    

This design incorporates rails on the outside of the Gantry.   Unlike the Tbstrong upgrade, this change will eliminate the interference with x axis movement and any cable chain system you might want to install.   The inside the gantry limits any well designed chain link system, as the adaptor off the tool head typically hits the rail on both gantry posts.

## 📦 Some basics to start wtih

- **This is an advanced mod adn not something to be taking lightly.   several different components are included in this modification and should only be done by someone with experience with complicated modifications**

- MGN12H rails are used, with the larger H carriages.

- Suggest to use light load Z rails, especially if you have a Beacon H or any other eddy probe. Any heavier preload will cause Z axis noise and cause the eddy to trigger early.

- There are prerequisites, you may want to consider. Initial release is designed to work with the SilencedFrost X axis rail upgrade and the Layer.Shifted double shear X motor upgrade.

- While changing the mount, consider an upgrade to a 48mm motor, over the 39mm on the stock Neptune 4 Pro. The standard motor will work.

- All files have included in this repo which were sourced from other mods, have been modified to work for this kit.   Including the printhead hanger for the x axis rail modification and modded to support the end stop switch being flipped from stock, requireing a  finger on top of the rail to activate the end switch

- The current offset on the x axis endstop switch is designed to fit the stock position, and the finger added to the x axis printhead will trigger a stock -8.5mm

## 🧰 Tools Required

- A working printer
- Hex drivers 2.5 and 2.0
- Soldering Iron (insert ends optional but recommended)

## 🛠️ Installation Overview

| Step | Instruction | Image |
|------|-------------|-------|
| 1 | **Print the STL files** using your Neptune 4 Pro or another 3D printer. | ![Step 1](image1.png) |
| 2 | **Disassemble** the original Z-axis lead screw carriage if necessary. This is self-explanatory, and there are no parts from the stock Z-axis hardware that are reused except for the limit switch. | ![Step 2](image2.png) |
| 3 | **Mount the linear rail** to the Z gantry using provided mounting holes and printed brackets. Use the `20x20x20` spacer block from the STL directory to position the 330mm rail. Tighten one rail screw, place the block on top, and align to the top of the gantry extrusion (with the top rail removed). This will give about 5mm of carriage travel before hitting the bed. Use roll-in T-nuts and M3x8mm screws spaced every other hole, starting with both ends. **DO NOT ADD THE CARRIAGES YET** — you will lose bearings if you try to install the assembly all at once. | ![Step 3](image3.png) |
| 4 | **Assemble the X-axis extrusion**. The X-axis brackets are designed for 2020 extrusion and not the stock one. The bracket mounting holes won’t align with stock extrusion holes. A future mod may support this. The X hangers use M4 T-nuts and allow vertical adjustment. Lower the assembly onto the gantry uprights, and use the X-axis leveling blocks to level. Leave all X extrusion screws loose for now; tighten them later after carriage alignment. | ![Step 4](image4.png) |
| 5 | **Attach the carriage**. With the X extrusion in place, slide the carriages onto the rails and into the hangers. Mount them to the X-axis bracket with 4× M3x8mm flat head screws. Slide the X axis up/down a few times. Then: 1) Tighten the top rail screw. 2) Loosen others. 3) Slide again. 4) Rest on leveling blocks. 5) Tighten screw nearest to X-axis on both rails. 6) Slide to bottom. 7) Tighten bottom screws. Finish by tightening remaining screws. | ![Step 5](image5.png) |
| 6 | **Tighten the X extrusion hangers**. Tighten the visible M4 screw in the X extrusion bracket using the access hole in the lead screw hanger. Remove the assembly from the gantry to access and tighten the hidden screw. **REMOVE THE CARRIAGES AGAIN**, reinstall onto the gantry extrusions, and repeat the carriage attachment instructions. Your motion system should now be aligned and level. | ![Step 6](image6.png) |
| 7 | **Mount assembly to the lead screw nuts**. Whether using stock nuts or Oldhams, now attach the lead screws. If using stock nuts: leave screws loose. If using Oldhams: tighten fully. | ![Step 7](image7.png) |
| 8 | **Mount your printhead and belt**. _Several options will need to be detailed here._ | ![Step 8](image8.png) |




## 📌 Compatibility

- **Printer:** Elegoo Neptune 4 Pro, will likely work on all Neptune versions, but not tested.   If not using a X axis endstop, the Motor side double shear cover would not be needed
- **X Axis and extrusion** currently only supported on a X rail upgrade from @SilencedFrost as referenced in the BOM above
- **X Axis motor and motion**  requires the Lamarc double shear upgrade.   It may be compatible with stock limit switch and cover, but not tested
- **Rail type:** MGN12H (or similar) with 330mm recommended length.  .step files provided to invite mods for longer x extrusions and mods like purge buckets outside the print area
- **Clearances:** Designed to maintain compatibility with stock frame dimensions.  

## 🧪 Notes

- **IMPORTANT** Files are designed with **tight tolerances** to minimize backlash and reduce resonance vibrations
- .step files are included so you can modify dimensions or hole patterns as needed
- Be sure to tune your flow and PA, there are very tight tollerances designed into the parts, and there will be no design to relax the tollerances
- Supports are built in, and desinged to be break-away after cooling.   Difficult to remove supports with hot/warm part
- ASA-CF does not seem to hold up to screw pressure to well.   As the screw head puts pressure on the assembly, the ASA catestophically fails and splits the parts.   PETG-GF can be used as alternative where screw pressure causes ASA to fail
- Socket head screws used where over tightening will not cause splitting


## 📦 BOM
<small>
  
| Item| Part Description                            | Quantity | Source/Link                             | Notes                                      |
|-----|---------------------------------------------|----------|------------------------------------------|--------------------------------------------|
| 1   | MGN12H Linear Rail (330mm)                  | 2        | [Amazon](https://www.amazon.com/dp/B07Z5NKF42)        | Light preload recommended                   |
| 2   | M3 x 8mm socket Head Screws                   | 16    | [Amazon](https://www.amazon.com/dp/B07CJ9BRCK?ref_=ppx_hzsearch_conn_dt_b_fed_asin_title_6&th=1)    | required for mounting the rails and a number of the printed components |
| 3   | M3 x 6 Flat head Screws                     | 8        | [Amazon](https://www.amazon.com/dp/B0CG9K1NDX?ref_=ppx_hzsearch_conn_dt_b_fed_asin_title_2) | Mounting the carraiges to the X axis brackets   |
| 4   | M3 x 8mm Button Head Screws                   | 4       | [Amazon](https://www.amazon.com/dp/B083HD61FV)                   | Mounting Lead screw hanger to the X axis bracket            |
| 5   | Gates Powergrip® 2GT Toothed Idler 20T              | 1        | [PrintedSolid](https://www.printedsolid.com/products/gates-powergrip-2gt-toothed-idler-5mm-id?variant=21236971241557)          |  upgraded to a gates spec on the X axis idler   |
| 6   | M3 x L4 x D4.2 Heat Insert  | <how many?>    |  [Amazon](https://www.amazon.com/dp/B0BBSLL6G7)  |  These are the small heat inserts
| 7   | M3 x L4 x D5 Heat Insert |<how many?> | [Amazon](https://www.amazon.com/dp/B0CS6VZYL8)    |  used for the heavier holding joints|
| 8   | M3 x 25 Socket Head Screw  |  2     |[Amazon](https://www.amazon.com/dp/B07NSX12DP)   |  mounting the tensioner cover to the X mounting bracket|
| 9   | M3 x 40 Socket Head Screw  | 4  |  [Amazon](https://www.amazon.com/dp/B0D5CQ5SX3)  | mounting the double shear cover to the base and motor.   Purchased a bundle instead of all independent  |
| 10  | M6 Gates GT2 belt    | 1  | [Amazon](https://www.amazon.com/dp/B08R93QQ8Z)  | new belt for futre extension of x axis length  |
| 11  | M5 x 20 steel Dowel  | 1   | [Amazon](https://www.amazon.com/dp/B07MB8QMT8)  | for the idler pulley  |
| 12  | M3 M3 Spring T Nut 2020 | <rails?>  | [Amazon](https://www.amazon.com/dp/B09H5B17GT)  | mounting the rails    |
| 13  | M4 Roll in T-Nut with Ball Spring| 4  | [Amazon](https://www.amazon.com/dp/B0D12GMX2Y)  |  mounting to the X extrusion  |
| 14  | 48mm Stepper Motor                          | 1        | [Moons Upgrade](https://www.aliexpress.us/item/3256805046302407.html?spm=a2g0o.order_list.order_list_main.16.211c18026A43A8&gatewayAdapt=glo2usa)        | This is not mandatory, but why go through all the upgrading and not upgrade the base motor       |
| 15   | SilencedFrost X-Axis Rail Upgrade           | 1        | [Github](https://github.com/SilencedFrost/Neptune-4-series-X-rail)        | Supporting Parts, Printhead back from here                      |
| 16   | Layer.Shifted X-Motor Double Shear Mount    | 1        | [Printables](https://www.printables.com/model/1222791-neptune-44pro-x-axis-double-shear-motor-upgrade)            | Source for some of the base files, remix included in this repo|

</small>

## 🛠️ Printing suggestions
- 0.4mm nozzle
- ASA-CF, PETG-GF, ASA or more rigid filaments.
- 0.2 layer height
- 0.45 layer width
- no supports, all necessary supports are built in
- Lead screw hangers printed with lead screw hole on build plate
- Double Shear parts printed with "cap" on plate - all parts with largest flat surface on plate
- Tensioner knob - not necessary, but included as a longer knob portion to account for camera hanger knob lock



## 🤝 Contributing

Improvements, remixes, or support for other printers are welcome!
Feel free to fork the repo and submit pull requests.

## 📜 License

This project is open source and licensed under the [MIT License](LICENSE).

## 🙌 Acknowledgments

Inspired by community mods for the Neptune and Ender series printers.

---

