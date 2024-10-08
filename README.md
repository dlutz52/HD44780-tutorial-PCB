# HD44780 Tutorial PCB

My inspiration for this PCB came from following Ian Ward's project on his web site:

[LCD2004 20×4 LCD Character Display with HD44780 Tutorial](https://excess.org/lcd2004-tutorial/)


![PCB Front Image](HD44780-tutorial-PCB-front.jpg)
![PCB Back Image](HD44780-tutorial-PCB-back.jpg)

# HD44780 Tutorial PCB BOM

## Wed, Mar 20, 2024, 05:20:29

## Component Count: 19

Ref | Qty | Value | Vendor\Part # | Description
----|-----|-------|---------------|-----------
C1, C2 | 2 | .01uF | Digikey\FG28C0G1H103JNT06 | Unpolarized capacitor 
D1 | 1 | RED | Generic | LED\3mm\Red 
D2 | 1 | BLUE | Generic | LED\3mm\Blue 
D3 | 1 | 8_SEG_LED  BAR_GRAPH (RED) | Generic | LED Bar Graph\Red\1x8 
D4 | 1 | GREEN | Generic | LED\3mm\Green 
D5 | 1 | YELLOW | Generic | LED\3mm\Yellow
J1 | 1 | PinSocket_1x16_P2.54mm_Vertical | Generic | Female Pin Header\1x16\2.54mm pitch
J2 | 1 | UJC-HP-M-G-5-MSMT-TR | Digikey\2223-UJC-HP-M-G-5-MSMT-TRDKR-ND | Type C/20 VDC/3A/Horizontal/6 Pin/Power Only
R1, R5, R6, R9 | 4 | 330ohm | Digikey\13-MFR-25FRF52-330RCT-ND | Resistor\330 Ohm\1%\1/4W\Axial
R2, R3, R4 | 3 | 1Kohm | Digikey\13-MFR-25FTE52-1KCT-ND | Resistor\1Kohm\1%\1/4W\Axial
R7, R8 | 2 | 5.1Kohm | Digikey\13-MFR-25FTE52-5K1CT-ND | Resistor\5K1ohm\1%\1/4W\Axial
RN1 | 1 | 470ohm | Digikey\4609X-101-471LF-ND | Resistor Array\ 8 Resistors\470ohm\9SIP
RN2 | 1 | 1Kohm | Digikey\4609X-101-102LF-ND | Resistor Array\ 8 Resistors\1Kohm\9SIP
RV1, RV2 | 2 | 5Kohm | Digikey\3386P-1-502LF | Trimmer Pot\5Kohms\0.5W\1/2W\Through Hole
S1 | 1 | TL2230 | Digikey\EG6031-ND | Switch\Pushbutton\DPDT\Through Hole
SW1 | 1 | REG SELECT | Digikey\450-1654-ND | Switch\Tactile\SPST-NO\0.05A\24V\Through Hole
SW2 | 1 | ENABLE | Digikey\450-1654-ND | Switch\Tactile\SPST-NO\0.05A\24V\Through Hole
SW3 | 1 | DS02C-254-1L-08BE | Digikey\2223-DS02C-254-1L-08BE-ND | Switch\Piano\8-DIP\SPST\25mA\24V\Through Hole

The LCD and its 16-pin male header are represented only with 3D models, but you need a 2004 LCD with a soldered 16-pin male header with a pitch of 2.54mm to plug into the 16 pin female header to complete this PCB. I have found the best place to get these is on eBay.

Do NOT try to use a 2004 LCD with an I<sup>2</sup>C adapter on it.

Most symbols/footprints/models are contained under the 'libraries' directory. Capacitors, resistors and LEDs use KiCad symbols/footprints/models.

KiCad 7.0.10 was used to create this PCB. KiCad 8.0.1 is out now and this project opens in that version. The newer KiCad will warn that this project was created in previous version and will be saved in a the newer format. When closing the schematic or a PCB just discard any changes. If you do not you will not be able to use KiCad 7 any more without difficulties.

Some models in KiCad's 3D view will display an appropriate socket under them but these can be omitted on the PCB - they are used to make it easier to replace any components should they need it in the future.
