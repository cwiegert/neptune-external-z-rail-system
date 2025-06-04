# Neptune 4 Pro – Z Axis Linear Rail Mounting System

This mod was inspired by the limitations and challenges imposed on Neptune printers by the TBStrong z rail kit.   Why do you need z rails at all?   Well, you don't, but I have them, and I never have to worry about aligning pom wheels, or any kind of z banding.   If you are here, you are interested in putting rails on the z axis, becuase you have probably already put the y axis rails and perhaps the x axis upgrade <link here for that git repo address>.    

This design incorporates rails on the outside of the Gantry.   Unlike the Tbstrong upgrade, this change will eliminate the interference with x axis movement and any cable chain system you might want to install.   The inside the gantry limits any well designed chain link system, as the adaptor off the tool head typically hits the rail on both gantry posts.

## 📦 Some basics to start wtih

- **This is an advanced mod and not something to be taking lightly.   Several different components are included in this modification and should only be done by someone with experience with complicated modifications**

- MGN12H rails are used, with the larger H carriages.

- Suggest to use light load Z rails, especially if you have a Beacon H or any other eddy probe. Any heavier preload will cause Z axis noise and cause the eddy to trigger early.

- There are prerequisites, you may want to consider. Initial release is designed to work with the SilencedFrost X axis rail upgrade  and the Layer.Shifted double shear X motor upgrade. 


- While changing the mount, consider an upgrade to a 48mm motor, over the 39mm on the stock Neptune 4 Pro.   The standard motor will work but if you are already doing this set of advanced modifications the motor upgrade is a nice add on

- All files have included in this repo which were sourced from other mods, have been modified to work for this kit.   Including the printhead hanger for the x axis rail modification and modded to support the end stop switch being flipped from stock, requireing a  finger on top of the rail to activate the end switch

- The current offset on the x axis endstop switch is designed to fit the stock position, and the finger added to the x axis printhead will trigger a stock -8.5mm
- **If you are using a tensioner idler pulley larger than a Gates Spec, be sure to print the Large profile tensioner housing**

## 🧰 Tools Required

- A working printer
- Hex drivers 2.5 and 2.0
- Soldering Iron (insert ends optional but recommended)

## 🛠️ Installation Overview

| Step | Instruction | Image |
|------|-------------|-------|
| 1 | **Print the STL files** using your Neptune 4 Pro or another 3D printer. | |
| 2 | **Disassemble** the original Z-axis lead screw carriage if necessary. This is self-explanatory, and there are no parts from the stock Z-axis hardware that are reused except for the limit switch. | ![Step 2](image2.png) |
| 3 |  Add a M3x8 socket head screw, starting with the top and bottom, every other hole, and start a roll in t-nut to the rail |  |
| 4 |  Using the bearing keeper from the tools, remove the carraiges from the linear rail by holding the keeper tight to the rail, and slowly sliding the carriages onto the bearing keeper |   |
| 5 | **Mount the linear rail** to the Z gantry.   Use the `20x20x20` spacer block from the STL directory to position the 330mm rail. Tighten one rail screw, place the block on top, and align to the top of the gantry extrusion (with the top rail removed). This will give about 5mm of carriage travel before hitting the bed. Snap the MGN12H alingment tool to the bottom of the rail and align the rail to the center of the extrusion.   Tighten the bottom screw tight enough to hold the rail.   Move the alignment clip between the top 2 holes of the rail, loosen the top screw, snap the alignment rail to the extrusion and tighten the top screw just past finger tight.  , tighten them just past finger tight, moving the alignment jig up the rail as you go.   **DO NOT ADD THE CARRIAGES YET** — you will lose bearings if you try to install the assembly all at once. | ![Step 3](image3.png) |
| 6 | **Assemble the X-axis extrusion**. The X-axis brackets are designed for 2020 extrusion and not the stock one. The bracket mounting holes won’t align with stock extrusion holes. A future mod may support this. Using 2 M4x10 button head screws and M4 roll in t-nuts, mount the X brackets to the extrusion.   Roughly align the carraige hanger portion of the bracket with the outside of the gantry rails.  Lower the assembly onto the gantry uprights, using the X-axis leveling jigs to maintain a level x axis.   Leave all X extrusion screws loose for now, they will be tighten after step 7 | ![Step 4](image4.png)  ![Step 6](image.png)|
| 7 | **Attach the carriage.** With the X extrusion in place, slide the carriages onto the rails and into the hangers. Mount them to the X-axis bracket with 4× M3x8mm flat head screws. Slide the X axis up/down a few times. Then:<br>&nbsp;&nbsp;&nbsp;&nbsp;1. Tighten the top rail screw.<br>&nbsp;&nbsp;&nbsp;&nbsp;2. Loosen other screws<br>&nbsp;&nbsp;&nbsp;&nbsp;3. Slide the X axis up and down again<br>&nbsp;&nbsp;&nbsp;&nbsp;4. Rest the X extrusion on the leveling blocks<br>&nbsp;&nbsp;&nbsp;&nbsp;5. Tighten screw nearest to X-axis on both rails<br>&nbsp;&nbsp;&nbsp;&nbsp;6. Slide the X extrusion to bottom of the rails<br>&nbsp;&nbsp;&nbsp;&nbsp;7. Tighten bottom screws<br>&nbsp;&nbsp;&nbsp;&nbsp;8. Finish by tightening remaining screws<br><br><br>   At this point the carraige and the rails should be aligned and parallel to each other and the x extrusion should move freely with little to no friction |  ![Step 5](image5.png) |
| 8 | **Tighten the X extrusion hangers**. Tighten the visible M4 screw in the X extrusion bracket using the access hole in the lead screw hanger. Remove the assembly from the gantry to access and tighten the hidden screw. Using the method described in step 4 **REMOVE THE CARRIAGES AGAIN**, repeat step 7 exactly. <br><br>Your motion system should now be aligned and level. | ![Step 6](image6.png) |
| 9 | **Mount assembly to the lead screw nuts**. Whether using stock nuts or Oldhams, attach the lead screws. If using stock nuts: leave screws loose. If using Oldhams: tighten fully. | ![Step 7](image7.png) |
| 10 | Slide the Printhead hanger onto the front rail.   Again, you will need to upgrade to the SilencedFrost front rail hanger system, or use a top rail from the TbStrong X axis rail system to use this upgrade.  There is no adapatation to the stock Neptune 4 Pro x extrusion.   Have not tested with the other Neptune 4 series. |  |
| 11 | Slide the motor into the receiver on the left side of the gantry.   The motor should be difficult to slide into the receiver, and best to slide the outside into the holder, then push the back of the motor towards the linear rail carraige | |
| 12 | Follow the assembly instructions from the Layer.shifted double shear block, to mount the bearing into the holder, and the end stop into the cap of the double shear holder |  |
| 13 | Slide your belt pulley onto the belt, leave the grub nut loose.  Pressure fit the double shear pulley assembly onto the motor hanger, and add the end stop mount to the assembly by inserting the 4 screws and start them into the motor.   Don't tighten them yet, just finger tight to hold the assembly together| |
| 14 |  Insert the pulley preload tool between the belt pulley and bearing of the double shear motor mount.   This tool aligns the pulley with the center of the x axis extrusion and gives enough standoff to avoid rubbing on the shaft reinforcement bearing. |  |
| 15 |  Assemble the tensioner by adding the heat insert and the M3x45mm screw to the back of the tensioner | |
| 16 |  Assemble the idler pulley in the tensioner using the M5x20mm dowel.   **If you are not using a Gates spec pulley, use the Large profile tensioner housing **  The tensioner slide will allow for 22mm dowel if you have 1 left over from another mod | |
| 17 | run the belt around the 2 pulleys and  making sure the tensioner pulley is onto the belt the correct way.   You will need to make sure the belt is around the tensioner pulley before mounting the pulley to the cover. |  |
| 18 | Slide the tensioner into the tensioner cover, and pressure fit the tensioner cover to the x axis mount adn tighten the 4 M3x35 socket head screws  |  |
| 19 | If you are using the c270 camera holer, add the mounting block prior to adding the tensioner nob.   There is no permanent mounting assembly for the block, it is loose fitting and held by the tension of the tensioner knob.   The teardop around the mounting hole will register into the profile on the end of the tensioner cover.   Add either the stock or the included tensioner knob and tighten slightly |  |
| 20 |  Tighten the belt to the print head hanger and assembly | |
| 21 |  Add the print head, and tune.   Tension the x belt to the appropriate tension (roughly 130 HZ for sock length Neptune 4 Pro)




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
| 6   | M3 x L4 x D4.2 Heat Insert  | 10    |  [Amazon](https://www.amazon.com/dp/B0BBSLL6G7)  |  These are the small heat inserts
| 7   | M3 x L4 x D5 Heat Insert | 6 | [Amazon](https://www.amazon.com/dp/B0CS6VZYL8)    |  used for the heavier holding joints|
| 8   | M3 x 25 Socket Head Screw  |  2     |[Amazon](https://www.amazon.com/dp/B07NSX12DP)   |  mounting the tensioner cover to the X mounting bracket|
| 9   | M3 x 40 Socket Head Screw  | 4  |  [Amazon](https://www.amazon.com/dp/B0D5CQ5SX3)  | mounting the double shear cover to the base and motor.   Purchased a bundle instead of all independent  |
| 10 | M3 x 45 Flat Head Screw | 1 | [Amazon](https://www.amazon.com/iexcell-Thread-Stainless-Socket-Screws/dp/B0CR6F4FQ2/ref=sr_1_3?crid=PM0GITL2CZU1&dib=eyJ2IjoiMSJ9.T676B9T6dQbunMhyRA0TNXkBoO-nPCkQ4SnpQQ6F3_4jmDoyINuJ31jmmUsZlpzi1LE6w-9rYqs60r2jXmNmnJ4QDKGnRYtXAhCVfWKc8MiLy-mtjGhuOznEJc83rtjNpP4i8G5F12gJgmq2mZMLoH2nYN7_Yi1MBiOkW0bhwjujedLfXf9vtfBdDc0MYfmeCQepIam53jqm8PsIsSr2cHTu5ZPISqoiEXly6OOTqn8.OS5zB21WLpXeArFbxTze_2pfss5rVPPspHQnTr4Alm4&dib_tag=se&keywords=m3+x+45mm+flat+head+screws&qid=1748998823&sprefix=m3+x+45mm+flat+head+screws%2Caps%2C154&sr=8-3) | mounting the tensioner knob |
| 10  | M6 Gates GT2 belt    | 1  | [Amazon](https://www.amazon.com/dp/B08R93QQ8Z)  | new belt for futre extension of x axis length  |
| 11  | M5 x 20 steel Dowel  | 1   | [Amazon](https://www.amazon.com/dp/B07MB8QMT8)  | for the idler pulley  |
| 12  | M3 Spring T Nut 2020 | 14  | [Amazon](https://www.amazon.com/dp/B09H5B17GT)  | mounting the rails    |
| 13  | M4 Roll in T-Nut with Ball Spring| 4  | [Amazon](https://www.amazon.com/dp/B0D12GMX2Y)  |  mounting to the X extrusion  |
| 14  | 48mm Stepper Motor (optional)                          | 1        | [Moons Upgrade](https://www.aliexpress.us/item/3256805046302407.html?spm=a2g0o.order_list.order_list_main.16.211c18026A43A8&gatewayAdapt=glo2usa)        | This is not mandatory, but why go through all the upgrading and not upgrade the base motor       |
| 15   | SilencedFrost X-Axis Rail Upgrade           | 1        | [Github](https://github.com/SilencedFrost/Neptune-4-series-X-rail)        | Supporting Parts, Printhead back from here                      |
| 16   | Layer.Shifted X-Motor Double Shear Mount    | 1        | [Printables](https://www.printables.com/model/1222791-neptune-44pro-x-axis-double-shear-motor-upgrade)            | Source for some of the base files, remix included in this repo|
| 17 | X axis extrusion leveler | 1 | [Printables](https://www.printables.com/model/680531-elegoo-neptune-4-pro-gantry-level/files)|Source files for the x axis levelers|
| 18 | Carriage block assembly helper | 2 | [Printables](https://www.printables.com/model/118195-mgn9-mgn12-blockcarriage-disassembly-helpers)| Source for bearing keeper|

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

## 🛠️ Modifications Ecouraged
- The step files are included to encourage creativity and modificaitons.   This is a starter pack and framework designed and implemented on a Neptune 4 Pro
- If you have suggestions, please add an issue, and I will consider adding the additions as user modifications.
- After enough beta testing, will consider making kit available on Printables.

## 🤝 Contributing

Improvements, remixes, or support for other printers are welcome!
Feel free to fork the repo and submit pull requests.

## 📜 License

This project is open source and licensed under the [MIT License](LICENSE).

## 🙌 Acknowledgments

Inspired by community mods for the Neptune and Ender series printers.

---

