# Starbie
A tiny motion controlled digital pet: a desktop tamagotchi that lives on a custom PCB. This version is a Kirby style pet that wanders a small OLED and reacted when ypu shake/tilt the board. It likes to stargaze when nothing is going on.

Built for Hack Club's Half-Life by following the guide.
<img width="893" height="683" alt="image" src="https://github.com/user-attachments/assets/e1341af4-e23a-4868-9d7b-78e07109b46e" />

# What it is
Starbie sits on your desk and shows its personality through the sall display. It also reacts to how you handle it. You can interact with it by oving the board. The board has a microcontroller, display, motion sensor, and environmental sensor in its PCB design. 

# What it does
- Wanders across the screen as a 32x32 px Kirby
- Radial menu: press Button 1, tilt the board as a selector ball, then press Button 1 again to pick an action. Each action changes the pet's stats
- Stats screen: Button 2 to see joy, energy, fullness
- Shake reaction: shake the board

# Cool features
- Sparkle trail behind the Starbie when it walks
- Idle stargazing: after 15 sec with no activity, Starbie stops and twinkling stars appear above it
- Custom Kirby sprite

# Hardware
- Seeed XIAO ESP32-C3:	Microcontroller
- SSD1306 128x64 OLED (I2C): Display
- MPU6050:	Motion sensor for the tilt menu and shake
- DHT11:	Temperature and humidity
- 2x tactile buttons:	Menu and stats

# Controls
- Button 1 (first press):	Open the radial menu
- Tilt (menu open):	Move the selector ball
- Button 1 (second press):	Choose the highlighted action
- Button 2:	Show or hide the stats screen
- Shake:	Starbie wiggles

# Software
Firmware/ contains one Arduino IDE sketch for the microcontroller. All settings are at the top. 

# Repo contents
- PCB/ - KiCad source files, schematic PDF, and fabrication exports (Starbie-gerbers.zip)
- Firmware/ - Arduino IDE sketch (Starbie/Starbie.ino)

# Credits
- Based on the Hack Club Half-Life Starbie guide
- Kirby is a character owned by Nintendo. This is a personal, non-commercial fan project.

