# Uriel
A 40% keyboard 
PCB - 
<img width="1171" height="423" alt="image" src="https://github.com/user-attachments/assets/a7ca9898-f372-4d5d-baa2-a13e4728031d" />

Schem-
<img width="815" height="662" alt="image" src="https://github.com/user-attachments/assets/d67b739e-a609-45c9-b734-875adbb11da1" />
<img width="1055" height="381" alt="image" src="https://github.com/user-attachments/assets/18422b5e-abdc-43f2-b54b-54e3b1ae4319" />
Bom
# Bill of Materials (BOM) - Custom 47-Key Split Ergo Keyboard

| #  | Component                  | Qty | Description / Specs                                                                 | Part / Model                          | Approx. Price (USD) | Source / Link                                                                 | Notes |
|----|----------------------------|-----|-------------------------------------------------------------------------------------|---------------------------------------|---------------------|-------------------------------------------------------------------------------|-------|
| 1  | Wireless Controller        | 2   | NRF52840 dev board, Nice!Nano v2 compatible, BLE + charging, Pro Micro footprint, headers | NRF52840 Nice!Nano alternative        | $4.34 each (~$8.68) | eBay (seller: survy2014) - https://www.ebay.com/itm/405014063318 | Use as `nice_nano_v2` in ZMK. Deep sleep ~1mA (higher than official ~20µA). |
| 2  | Keyboard Switches          | 90| Akko Rosewood Linear, 5-pin MX-compatible, 40gf, factory lubed, deep/low-pitch     | Akko Rosewood (45 pcs/box)            | $29.46 / 45 pcs     | AliExpress - AKKO Official Store (https://www.aliexpress.com/item/1005007227966289.html) | yep need 90 cuz I have 47 switches also will use these in my next project 60% keeb.|
| 3  | Switching Diodes           | 50  | 1N4148                                  | 1N4148 pack                           | ~$2–$3 total        |(https://www.mouser.com/ProductDetail/onsemi/1N4148TR?qs=i4Fj9T%2FoRm%252BOzV8sfXrhvQ%3D%3D)                        | 1 per key (D1–D47 in schematic) + spares. Col2row orientation. |
| 4  | Reset Tactile Switch       | 2   | Right-angle, grounding, 6mm tact, SPST-NO                                          | MJTP1117 (Apem)                       | $0.61 each (~$1.22) | Mouser - [642-MJTP1117](https://www.mouser.com/ProductDetail/642-MJTP1117)   | SW2 in schematic, one per half. |
| 5  | Controller Socket Pins     | ~48 pins (or 4 strips) | Mill-Max low-profile sockets for Pro Micro/Nice!Nano footprint                     | 315-43-112-41-003000 (or equiv.)      | ~$2.80–$5           |                                                      | For easy controller swap/debug. Use 12-pin rows × 2 per side. |
| 6  | Extra IC Socket Pins       | 30+ | Mill-Max standard pins for misc (I2C header J1, etc.)                              | 03320-000-15-000-003-0 (or similar)   | ~$2.28 for 30       | Mouser [your screenshot]                                                      | For J1 (SDA/SCL/VCC/GND) if adding OLED/rotary. |
| 7  | LiPo Battery               | 2   | 3.7V 2000mAh with JST connector                                                    | EHB Lithium Polymer 2000mAh 105454A   | $11.99 each (~$24)  |                                                         | One per half; connect to JST (BAT+/GND). |
| 8  | Case / Dampening Foam      | 1–2 sheets | 3mm PORON/IXPE foam, black                                                         | MEARCOOH Premium Foam 3mm             | ~$9.96              |                                                        | For sound dampening inside case. |
| 9  | Misc Hardware              | Various | Standoffs, M2 screws/nuts, brass coupling nuts, silicone bumpers/rings, O-rings   | Assorted (e.g., Harfington rings, Juminiz bumpers) | ~$30–$40 subtotal   | <img width="479" height="894" alt="image" src="https://github.com/user-attachments/assets/fe4f18eb-0bc6-405a-95e1-58d8b1236350" />
                          | Includes PCB standoffs, door bumpers, etc. |
| 10 | Hotswap Sockets  | 50 | Kailh MX hotswap sockets                                                           | Kailh hotswap socket pack             | ~$10–$15            | (https://www.amazon.com/Hot-swap-CPG151101S11-Mechanical-Keyboard-Accessories/dp/B0BVH6M5FP/ref=sr_1_2?crid=185WUZGQMJURM&dib=eyJ2IjoiMSJ9.4jfJMBrnUtVfrD9ndIz5Dbi40PLToNJ99BfeLn_g7eC3as9_vrQNvkGyA0VYvWPXLxbbf6z5IqYGKoKjoGVQ2Tqd2B5bLg4LBKhudEK4Hkn1NNJmjkN55wIJhqDrLLQxOgRPxAMQSmebKoSGv4Lc917p-XXNpmHUKGWYyTnOEItFdfpEvkFigntOmWAuBSDsbIioWwjYtbuR8FoSlRWeT9nHoz-EYGd4OoI5ynr3pLw.X1o5-P5xyYim82wC0a1vmnchDTXbSWMIpJfHheI6knw&dib_tag=se&keywords=hot%2Bswap%2Bkailh%2Bsockets&qid=1769058366&sprefix=hotswap%2Bkalih%2Bsocket%2Caps%2C226&sr=8-2&th=1)                              | If not soldering switches directly. |
| 11 | Keycaps      | 1   | Doublshot pbt keycaps                                             | Keycaps                  | $13              |(https://www.amazon.com/gp/product/B0D1JWX3PP/ref=ox_sc_act_title_1?smid=AFB5KTL5FE772&psc=1)                                                                    | |

