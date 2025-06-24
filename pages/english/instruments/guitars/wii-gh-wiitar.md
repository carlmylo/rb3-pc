---
title: Nintendo Wii Guitar Hero Guitars (WiitarThing)
sidebar: controllers_sidebar
permalink: ctrls_ghwtrgtr_wii
folder: instruments
tags: [wii, guitars, english]
summary: "How to setup Nintendo Wii Guitar Hero guitars using WiitarThing on RPCS3."
toc: false
---

<div align="center"> <img src="https://rb3pc.milohax.org/images/instruments/plat/wii.png" alt="Platform" title="Platform"></div>

<div align="center"> <img src="https://rb3pc.milohax.org/images/instruments/cont/wiighgtrscontroller.png" alt="Controller" title="Controller"></div>

## NOTES

* Requires installing and running [[**WiitarThing**]](https://github.com/TheNathannator/WiitarThing){:target="_blank"} along with its dependencies.
* This configuration **requires connecting wirelessly via Bluetooth**. You need a Bluetooth receiver to connect to your computer.
    * It's suggested to mod your guitar into a wired one with a solution like [[a V3 adapter by RetroCultMods]](https://shop.retrocultmods.com/products/v3-wii-adapter-for-clone-hero-and-rb4-rock-band-4){:target="_blank"}. a [[Revival Kit from RetroCultMods]](https://shop.retrocultmods.com/products/revival-kit-for-guitar-hero-controllers-by-retrocultmods){:target="_blank"}, or a [[Solderless DIY RGB Kit from RetroCultMods]](https://shop.retrocultmods.com/products/solderless-diy-rgb-kit-for-guitar-hero-controllers-by-retrocultmods){:target="_blank"}.
* **Tilt is busted on this controller!**
* RPCN Menus (for sending or accepting online invites) may cause a softlock. You may need an alternative input method to navigate these menus, such as [[a typing keyboard or a gamepad]](https://rb3pc.milohax.org/ctrls#gamepads){:target="_blank"}.

## Initial Setup

1. After installing [[WiitarThing]](https://github.com/TheNathannator/WiitarThing/releases){:target="_blank"} along with [[ViGEmBus]](https://github.com/nefarius/ViGEmBus/releases){:target="_blank"}, open it up.

2. Press the **`[SYNC]`** button at the top left.  
![A screenshot of WiitarThing with a cursor hovering over the red "SYNC" button.](https://rb3pc.milohax.org/images/instruments/xtra/wiitar/wiitarsyncbut.png "WiitarThing v2.7.0.5")

3. Press either the red `SYNC` button on the back of your Wii Remote<sup>a</sup> or press both `1+2` at the same time<sup>b</sup>. You may have to try this a few times.  
<sup>a</sup>  
![A Wii Remote with the 1 and 2 buttons being highlighted.](https://rb3pc.milohax.org/images/instruments/xtra/wiitar/wiimotesync12.gif "Wii Remote")  
<sup>b</sup>  
![A Wii Remote with the "SYNC" button the back being highlighted.](https://rb3pc.milohax.org/images/instruments/xtra/wiitar/wiimotesyncbut.gif "Wii Remote")

4. Once it's synced, click **`[CONNECT]`**.  
![A screenshot of WiitarThing with a cursor hovering over the "CONNECT" button.](https://rb3pc.milohax.org/images/instruments/xtra/wiitar/wiitarconnectbut.png "WiitarThing v2.7.0.5")

5. Open RPCS3's `Pads` menu.

<!-- Map Start -->
<div class="panel-group" id="accordion">
                    <div class="panel panel-default">
                        <div class="panel-heading">
                            <h4 class="panel-title">
                                <a class="noCrossRef accordion-toggle" data-toggle="collapse" data-parent="#accordion" href="#how-to-map-pads">How do I map my guitar?</a>
                            </h4>
                        </div>
                        <div id="how-to-map-pads" class="panel-collapse collapse noCrossRef">
                            <div class="panel-body">
<ul>
<p><strong>Click on the Pads icon at the top of RPCS3</strong>.</p>
<p><img src="https://rb3pc.milohax.org/images/instruments/rpcs3pad.png" alt="A screenshot of RPCS3, showing the cursor over the Pads menu." title="Pads"></p>
<p>It’s suggested to create a new configuration by clicking <code>Add Configuration</code> at the top right of the <code>Pads</code> window.<br>
This is so you can change configuration profiles in case you want to play games that don’t use instruments.<br>
<img src="https://rb3pc.milohax.org/images/instruments/rpcs3padprofadd.png" alt="A screenshot of the top right of RPCS3's Pads window. &quot;Add Configuration&quot; is being clicked on by the mouse cursor." title="Add Configuration"></p>
<p>Follow the instructions and/or match the assignments below.</p>
<p><img src="https://rb3pc.milohax.org/images/instruments/padlegend.png" alt="A picture showing how the instrument page and RPCS3 can be used as a mapping reference." title="Mapping the Rock Band Hofner"></p>
</ul>
                            </div>
                        </div>
                    </div>
</div>
<!-- Map End -->

## Pad Information

| Handlers | Devices |
|:--------:|:-------:|
| XInput | XInput Pad |

| Device Class | Device Subtype |
|:------------:|:--------------:|
| Guitar | Guitar Hero |

## Mapping

By default, XInput has most things bound correctly. You only need to adjust the following:

**UNMAP THE FOLLOWING** or guitar solos will auto-strum!  
Use Right Click to unmap a button.

| **RPCS3** | **XInput** | **Guitar** |
|:--------:|:-----------:|:-----------:|
| L2 | ![Left Trigger](https://rb3pc.milohax.org/images/btns/ctrls/360/lt.png "Left Trigger") | Solo Modifier |

**Change the following** or blue and yellow frets will be inverted!

| **RPCS3** | **XInput** | **Guitar** |
|:--------:|:-----------:|:-----------:|
| Square | ![Y Button](https://rb3pc.milohax.org/images/btns/ctrls/360/y.png "Y Button") | ![Yellow Fret](https://rb3pc.milohax.org/images/btns/gtrs/yf.png "Yellow Fret") | 
| Triangle | ![X Button](https://rb3pc.milohax.org/images/btns/ctrls/360/x.png "X Button") | ![Blue Fret](https://rb3pc.milohax.org/images/btns/gtrs/bf.png "Blue Fret") |

Guitar Hero controllers tend to misbehave and **refuse to map sometimes. If you try mapping a button and always get "U+" or something similar, click "Filter Noise"** at the bottom left of the controller configuration window **then try mapping**.

<div class="panel-group" id="accordion">
                    <div class="panel panel-default">
                        <div class="panel-heading">
                            <h4 class="panel-title">
                                <a class="noCrossRef accordion-toggle" data-toggle="collapse" data-parent="#accordion" href="#advanced-mapping">Advanced Mapping</a>
                            </h4>
                        </div>
                        <div id="advanced-mapping" class="panel-collapse collapse noCrossRef">
                            <div class="panel-body">
<h4 id="profile">Profile</h4>
<p><a href="https://github.com/hmxmilohax/rb3-pc/raw/refs/heads/main/downloads/instrument-repo/Nintendo%20Wii%20Guitar%20Hero%20Wiitar%20Thing.7z">[Download Profile]</a></p>
<div class="alert alert-info"><i class="fa fa-info-circle"></i> <b>This is not recommended if you're using multiple controllers at once. </b> {{include.content}}</div>
<p>After downloading the profile,</p>
<ol>
<li>Extract the .7z file.</li>
<li>Drag the <code>input configs</code> folder into the <code>configs</code> folder where you have RPCS3 in.</li>
</ol>
<p><img src="https://rb3pc.milohax.org/images/instruments/instrepoinstall.gif" alt="A GIF of a user dragging the Wii Rock Band Guitar configuration into their RPCS3 folder." title="Installing a configuration from the Instrument Repo"></p>
<p>After that, you can select the profile in the <strong>“Pads”</strong> menu.</p>
<p><img src="https://rb3pc.milohax.org/images/instruments/rpcs3padprofile.png" alt="A screenshot of RPCS3's Gamepad Settings, showing the cursor over a profile." title="Gamepad Settings"></p>
<p>Most of the time, these controller profiles should work out of the box. If they don’t, try changing the controller listed in “<code>Devices</code>”, next to the “<code>Refresh</code>” button until it receives an input. You can edit this while the game is running.</p>
<h4 id="profile">Bindings</h4>
<table>
<thead>
<tr>
<th align="center"><strong>RPCS3</strong></th>
<th align="center"><strong>Guitar</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td align="center">Cross</td>
<td align="center"><img src="https://rb3pc.milohax.org/images/btns/gtrs/gf.png" alt="Green Fret" title="Green Fret"></td>
</tr>
<tr>
<td align="center">Circle</td>
<td align="center"><img src="https://rb3pc.milohax.org/images/btns/gtrs/rf.png" alt="Red Fret" title="Red Fret"></td>
</tr>
<tr>
<td align="center">Square</td>
<td align="center"><img src="https://rb3pc.milohax.org/images/btns/gtrs/yf.png" alt="Yellow Fret" title="Yellow Fret"></td>
</tr>
<tr>
<td align="center">Triangle</td>
<td align="center"><img src="https://rb3pc.milohax.org/images/btns/gtrs/bf.png" alt="Blue Fret" title="Blue Fret"></td>
</tr>
<tr>
<td align="center">L1</td>
<td align="center"><img src="https://rb3pc.milohax.org/images/btns/gtrs/of.png" alt="Orange Fret" title="Orange Fret"></td>
</tr>
<tr>
<td align="center">D-Pad: Up</td>
<td align="center"><img src="https://rb3pc.milohax.org/images/btns/gtrs/sbu.png" alt="Strumbar Up" title="Strumbar Up"></td>
</tr>
<tr>
<td align="center">D-Pad: Down</td>
<td align="center"><img src="https://rb3pc.milohax.org/images/btns/gtrs/sbd.png" alt="Strumbar Down" title="Strumbar Down"></td>
</tr>
<tr>
<td align="center">D-Pad: Left</td>
<td align="center"><img src="https://rb3pc.milohax.org/images/btns/gtrs/dpl.png" alt="D-Pad: Left" title="D-Pad: Left"></td>
</tr>
<tr>
<td align="center">D-Pad: Right</td>
<td align="center"><img src="https://rb3pc.milohax.org/images/btns/gtrs/dpr.png" alt="D-Pad: Right" title="D-Pad: Right"></td>
</tr>
<tr>
<td align="center">Right Stick: <br> Left/Right</td>
<td align="center"><img src="https://rb3pc.milohax.org/images/btns/gtrs/wb.png" alt="Whammy Bar" title="Whammy Bar"></td>
</tr>
<tr>
<td align="center">Select</td>
<td align="center"><img src="https://rb3pc.milohax.org/images/btns/gtrs/ts.gif" alt="Tilt" title="Tilt Vertical"></td>
</tr>
<tr>
<td align="center">Select</td>
<td align="center"><img src="https://rb3pc.milohax.org/images/btns/gtrs/ts.gif" alt="Tilt" title="Tilt Horizontal"></td>
</tr>
<tr>
<td align="center">Start</td>
<td align="center"><img src="https://rb3pc.milohax.org/images/btns/ctrls/wii/plu.png" alt="Plus" title="Plus"></td>
</tr>
<tr>
<td align="center">Select</td>
<td align="center"><img src="https://rb3pc.milohax.org/images/btns/ctrls/wii/back.png" alt="min" title="Minus"></td>
</tr>
<tr>
<td align="center">PS Button</td>
<td align="center"><img src="https://rb3pc.milohax.org/images/btns/ctrls/wii/home.png" alt="Home" title="Home"></td>
</tr>
</tbody>
</table>
                            </div>
                        </div>
                    </div>
                    <!-- /.panel -->
</div>
<!-- /.panel-group -->

<div align="center"> <img src="https://rb3pc.milohax.org/images/instruments/maps/gtrwiiwtarmapping.png" alt="Mapping" title="Mapping"></div>

[[Back to Controllers]](https://rb3pc.milohax.org/ctrls#instrument-list)

Mapped by [[gonakil1ya]](https://gonakillya.neocities.org){:target="_blank"}
