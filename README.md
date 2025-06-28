# Butterfly Charm

This is a very simple butterfly charm which is basically a light up trinket that you can hopefully attach to your bag.
It features large vias for keychains.
The LEDs only turn on when it is dark outside, preserving battery power and becoming more eye-catching in the dark.
The circuit uses a photoresistor in tandem with a transistor to determine whether or not it is light outside.
When there is light, the photoresistor decreases in resistence, therefore lowering electron flow to the base gate of the transistor, preventing the 2 LEDs from getting enough current to significantly light up.
When there is no light, the resistence in the photoresistor increases, therefore more current flows through the base gate (around 0.05miliamps) allowing 5 miliamps to run the LEDs.
Red LEDs were used because they need the least current.

Slack username: Xinyang Wang

## BOM

| Item                | Qnt |
| ------------------- | --- |
| LEDs                | 2   |
| Battery holder 3034 | 1   |
| Photoresistor       | 1   |
| 220ohm resistors    | 2   |
| 100kOhm resistors   | 1   |
| NPN transistor      | 1   |
| PCB                 | 1   |

## Images

![Schematic](img/schematic.png)
![PCB](img/pcb.png)
![Front](img/front.png)
![Back](img/back.png)

## Thoughts

This was my first time designing a board using Kicad so it's a bit rough around the edges.
Getting the bezier curves to work was especially annoying and it took several iterations to smooth out the lumps.
There's probably a way to make an SVG the (Edges.Cuts) layer instead of having to polyline/curve it out but I'm too lazy to find out how.
The electronics are really simple. It's just connecting togther a battery, a LED, a resistor and a button.
Not much to explain. In fact, the most challenging part was designing the butterfly shape in Krita and getting the pattern on the back to work.
Oh hopefully the comically large vias won't destroy the structural stability of the part because I actually plan on using this.
If I have any advice for other people, it's to not use Kicad with a tiling window manager. It made things really difficult.
Also I almost forgot to run the checker. I just realized that my button holes weren't actually connected to the copper trace beneath them.
Hopefully nothing else is broken...
