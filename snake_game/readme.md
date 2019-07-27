Found this snake game and 6502 assembly tutorial on https://skilldrick.github.io/easy6502/

Notes on how his Javascript emulator works (that we have to mimic)

Memory location $fe contains a new random byte on every instruction.
Memory location $ff contains the ascii code of the last key pressed.

Memory locations $200 to $5ff map to the screen pixels. Different values will
draw different colour pixels. The colours are:

$0: Black
$1: White
$2: Red
$3: Cyan
$4: Purple
$5: Green
$6: Blue
$7: Yellow
$8: Orange
$9: Brown
$a: Light red
$b: Dark grey
$c: Grey
$d: Light green
$e: Light blue
$f: Light grey

The screen is 32 pixels wide
The screen is 32 pixels tall

$200 0,0 is top left
$21f 31,0 is top right
$5e0 0,31 is bottom left
$5ff 31,31 is bottom right

