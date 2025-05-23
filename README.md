# Neptune 4 Pro – Z Axis Linear Rail Mounting System

This mod was inspired by the limitations and challenges imposed on Neptune printers by the TBStrong z rail kit.   Why do you need z rails at all?   Well, you don't, but I have them, and I never have to worry about aligning pom wheels, or any kind of z banding.   If you are here, you are interested in putting rails on the z axis, becuase you have probably already put the y axis rails and perhaps the x axis upgrade <link here for that git repo address>.    

This design incorporates rails on the outside of the Gantry.   Unlike the Tbstrong upgrade, this change will eliminate the interference with x axis movement and any cable chain system you might want to install.   The inside the gantry limits any well designed chain link system, as the adaptor off the tool head typically hits the rail on both gantry posts.

## 📦 Some basics to start wtih

- MGN12H rails are used, with the larger H carriages.

- Suggest to use light load Z rails, especially if you have a Beacon H or any other eddy probe. Any heavier preload will cause Z axis noise and cause the eddy to trigger early.

- There are prerequisites, that you may want to consider. Initial release is designed to work with the SilencedFrost X axis rail upgrade and the Layer.Shifted double shear X motor upgrade.

- While changing the mount, I upgraded to a 48mm motor, over the 39mm on the stock Neptune 4 Pro. The standard motor will work - but I had an extra, so why not.

- All files have included in this repo which were sourced from other mods, have been modified to work for this kit.   Including the printhead hanger for the x axis rail modification.   Because the end stop switch is flipped from stock, a finger on top of the rail was required for in this mod

- The current offset on the x axis endstop switch is designed to fit the stock position, and the finger added to the x axis printhead will trigger a stock 0 point.

- **finish writing the pre-reqs here... make sure to put the basics up top**

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

## 🧰 Tools Required

- 
- 
- 

## 🛠️ Installation Overview

1. **Print the STL files** using your Neptune 4 Pro or another 3D printer.
2. **Disassemble** the original Z-axis lead screw carriage if necessary.   This is self expanatory, and there are no parts from the stock z axis hardware that is reused except for limit switch
3. **Mount the linear rail** to the Z gantry using provided mounting holes and printed brackets.   **DO NOT ADD THE CARRAIGES**   If you add the carraiges first, YOU WILL LOSE bearings when you attempt to slide the entire assembly onto the rails  <will detail more here>
4. **Assemble the X axis extrusion**  The X axis brackets are designed to fit a 2020 extrusion and for not, not designed for the stock extrusion.   Future will add X hangers for the stock extrusion.   However
   the x hangers are built to use 4mm T-nut hangers and be adjusted after lowering the assembly onto the gantry upgrights.   Use the x axis leveling blocks to ensure your axis is level and leave all the X extrusion
   mounting screws loose.   You will tighten them after attaching the carraiges.   
5. **Attach the carriage**  Once the X extrusion is in place, slide the carraiges  onto the rails, and into the hangers after the assembly.  Mount them to the X axis bracket with the 4 x M3x8 flat head screws and tighten the carraiges
   Slide the X axis up and down a couple times.   When installing, I usually tighten the top screw of the rails, loosen all the others, and start tightenging the rail after this sliding motion.   After this sliding motion, rest
   the axis on the leveling blocks again, and tighten the screw on each rail which is closest to the X axis.   Then slide the X axis to the bottom, tighten the bottom rail screw, and proceed to tighten all remaining rail screws.  
6. **Tightening the X extrusion hangers**   Now it's time to tighten the exposed screw on the X extrusion bracket.   A hole in the lead screw hanger will give you access to the M4 mounting screw.   Tighten the 1, and remove the entire
    entire assembly from the gantry and tighen the screw which is hidden behind the gantry extrusion.      **REMOVE THE CARRAIGES**, yes, you have to remove the carraiges again, and reload the assembly onto the gantry extrusions.  Then, follow the instructions to attach the carraiges.   Your motion system should now be aligned and level
7. **Mount Assembly to the Lead Screw Nuts** whether you're using stock lead screw nuts, or Oldhams, now is the time to attach the lead screws to the system.   assemble as you normally would, with the screws being loose on on the stock nut, and tight if you're using Oldham's.
8.  **Mount your printhead and belt**  _several options will need to be detailed here_


## 📌 Compatibility

- **Printer:** Elegoo Neptune 4 Pro, will likely work on all Neptune versions, but not tested.   If not using a X axis endstop, the Motor side double shear cover would not be needed
- **X Axis and extrusion** currently only supported on a X rail upgrade from @SilencedFrost as referenced in the BOM above
- **X Axis motor and motion**  requires the Lamarc double shear upgrade.   It may be compatible with stock limit switch and cover, but not tested
- **Rail type:** MGN12H (or similar) with 330mm recommended length
- **Clearances:** Designed to maintain compatibility with stock frame dimensions

## 🧪 Notes

- Files are designed with **tight tolerances** to minimize backlash.
- STEP files are included so you can modify dimensions or hole patterns as needed.
- Be sure to tune your flow and PA, there are very tight tollerances designed into the parts, and there will be no design to relax the tollerances
- Supports are built in, and desinged to be break-away after cooling.   Difficult to remove supports with hot/warm part
- ASA-CF does not seem to hold up to screw pressure to well.   As the screw head puts pressure on the assembly, the ASA catestophically fails and splits the parts
- Socket head screws used where over tightening will not cause splitting
- 

## 🛠️ Printing suggestions
- 0.4mm nozzle
- ASA-CF, PETG-GF, ASA or more rigid filaments.
- 0.2 layer height
- 0.45 layer width
- no supports, all necessary supports are built in
- Lead screw hangers printed with lead screw hole on build plate
- Double Shear parts printed with "cap" on plate - all parts with largest flat surface on plate
- Tensioner knob - not necessary, but included as a longer knob portion to account for camera hanger knob lock
- 


## 🤝 Contributing

Improvements, remixes, or support for other printers are welcome!
Feel free to fork the repo and submit pull requests.

## 📜 License

This project is open source and licensed under the [MIT License](LICENSE).

## 🙌 Acknowledgments

Inspired by community mods for the Neptune and Ender series printers.

---

