# Mini Theremin with NE555

This is a small instrument that changes its sound depending on the light. It uses an 8-pin NE555 timer and a photoresistor. When I move my hand over the photoresistor, the shadow changes the pitch.

## How it works

The NE555 generates a signal that makes the piezo produce sound. The photoresistor changes its resistance depending on how much light hits it, which changes the frequency of the signal.

## Parts

| Part | Quantity |
|---|---:|
| NE555 in a DIP-8 package | 1 |
| 10 kΩ resistor | 2 |
| 10 nF capacitor | 2 |
| 100 nF capacitor | 1 |
| Photoresistor (LDR) | 1 |
| Passive piezo element | 1 |
| 2-pin connector | 3 |
| DIP-8 socket (optional) | 1 |

It also needs a 5 V power supply.

## Connectors

- J1 — power: pin 1 is +5V, pin 2 is GND.
- J2 — photoresistor.
- J3 — passive piezo element.

## PCB

I designed the schematic and PCB in KiCad 10. The PCB has no unconnected pads according to DRC. The photoresistor and piezo connect through separate headers, so they can be placed away from the board.

For the best effect, shine some light on the photoresistor and move your hand over it.

## Status

The PCB is designed, but it still needs to be manufactured and tested. Once it's assembled, I'll see how well it works and whether anything needs changing.
