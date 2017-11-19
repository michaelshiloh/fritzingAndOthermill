# fritzingAndOthermill



# A trivial single sided Arduino shield
Schematic

## Fritzing Instructions

    Open Fritzing and go to the Schematic View

    All components are in “Core Parts”

    IMPORTANT: Use only through-hole components (THT) (Through-Hole
Technology)

    From the section headed “Microcontrollers” select the first item which is
an Arduino Uno

    Add your LED (“Output”) and resistor  (“Basic”)

    Add another resistor (“Basic”) and the Force Sensitive Resistor (“Input”)

    Switch to the PCB View

    Select the grey outline

    In the Properties area of the Inspector, in the Layers field, select “One
layer (single sided)

    Just below the Layers field, in the Shape field, select “Arduino shield”

    Align the shape of the board with the shield template

    Move your components to the desired place

    IMPORTANT: All components must be on the top

    Add traces as necessary

    The default traces in Fritzing are quite thin and have a tendency to tear
off the PCB. Wherever possible, make the traces as wide as possible.

    IMPORTANT: All traces must be on the bottom

    When you are finished laying out your PCB, export your files:

        Empty a thumbdrive or create a new empty folder. Otherplan gets
confused if more than one project is present

        Export from Fritzing: File -> Export -> For production -> Extended
Gerber

        Put all the project files on the thumbdrive

## Othermill Instructions

### Preparation

1. If Otherplan is running, quit

1. Start Bantam software

1. Turn on Othermill

1. Home the machine

### Material

1. Single Sided FR-1 L2

1. Standard dimensions (5.000in X 4.000in Y 0.061in Z)

1. Select left or right bracket as appropriate

### Plans

1. Insert thumb drive

1. Click "Open Files"

1. Navigate to your thumb drive and select
	your copperTop.gtl file

1. "Choose Gerber Files" 

1.1. leave Top, Bottom, and Holes as is 

1.1.  click "Clear" for Outline

1.1.Press "Okay"

1. Your files will appear and you can see the board in the preview.

#### Parts to Mill

1. Note whether the preview is showing the right side of the board. If not,
select "Top" or "Bottom" in "Parts to Mill"

#### Placement

1. If the placement is not where you want it (e.g. if you are using a 
scrap of board) select "Placement" and move the board to where you want.
Always leave at least .1" between the bracket and your traces by placment
adjustment.

#### Milling Tools

1. add 1/16″, 1/32″, and 1/64″ Flat End Mill. The order doesn't matter.

Important: Now that you have added tools, OtherPlan will show the cuts it
will make. Inspect the board carefully and make sure that no traces or holes
are connected where they shouldn’t be, for example if they are too close
together

## Click "Mill all Visible"

1. You will be prompted to insert the smallest endmill

1.1. Insert the requested endmill

1.1. Close the window and press "Continue"

1.1. Press "Locate Tool"

1. You will be prompted to insert the next endmill

1.1. Insert the requested endmill

1.1. Close the window and press "Continue"

1.1. Press "Locate Tool"

1. Repeat for the next tool


        When the milling stops, move the board to the front of the machine
(Click “Loading” in “Move to Position”) and remove your board. There is a thin
spatula that can be used to help unstick your board.

# A double sided Arduino shield

Schematic

74HC4052_74HC595Shield_schem
Fritzing Instructions

    Open Fritzing and go to the Schematic View

    From the section headed “Microcontrollers” select the first item which is
an Arduino Uno

    Search for “595” and select the fourth item, the shift register from
Sparkfun

    Search for “4052” and select the third item, the analog mux from Sparkfun

    Switch to the PCB View

    Select the grey outline

    In the Properties area of the Inspector, in the Layers field, select “Two
layers (double sided)

    Just below the Layers field, in the Shape field, select “Arduino shield”

    Align the shape of the board with the shield template

    Move your components to the desired place

    IMPORTANT: Use only through-hole components (THT) (Through-Hole
Technology)

    Most components should be on the top. If you have any components on the
bottom think carefully about the pin order.

    The default traces in Fritzing are quite thin and have a tendency to tear
off the PCB. Wherever possible, make the traces as wide as possible.

    IMPORTANT: Think carefully about which side a trace will be soldered to a
component. Since most components are on the top, most soldering will take
place on the bottom, so most traces must connect to components on the bottom.

    Try to get all the traces on the bottom layer. If you must use traces on
the top to cross over lines, do not use any of the component holes. Instead
use vias, and select “Home Etched Via” under Hole Size

    IMPORTANT:

    When you are finished laying out your PCB, export your files:

        Empty a thumbdrive or create a new empty folder. Otherplan gets
confused if more than one project is present

        Export from Fritzing: File -> Export -> For production -> Extended
Gerber

        Put all the project files on the thumbdrive

Othermill Instructions

    If Otherplan is running, quit

    Start Otherplan

    Turn on Othermill. This may require both the power switch in the rear and
turning the red emergency stop button on the right hand side

    If you get a window that says “New network interfaces have been detected”
hit “Cancel”

    Home the machine

    Insert thumb drive

    Import files

        It will only allow you to click on your copperTop.gtl file but it will
import all the files

        (Optional step: If you did not select an outline for your circuit
board in Fritzing, select “Autogenerate” for the “Board Outline” setting. This
is at the bottom of the File Import window. If you don’t see the options,
click the “Options” button.)

    The first file loaded will be the top of your circuit board. It’s wise to
verify with your design in Fritzing that the correct side has loaded.

    Tell Otherplan to place this on the top side. Do this in the “Side:”
setting near the top right corner of the screen, in the “setup” section.

    Click “Loading” (in “Move to Position”)
    Insert double sided stock. Align the PCB  to the forward left corner of
the bracket.

    Set up material (in “Setup”)

        Double Sided FR-1 L2

        Standard dimensions (5.000in X 4.000in Y 0.061in Z)

        Click “Continue”

        Click “Align to Bracket”

        Click “Done

    Add tools

        In “Tools to Use” add 1/16″, 1/32″, and 1/64″ Flat End Mill

    Change tool

        Click “Change” in “Setup” next to Tool

        Remove end mill

        Click “Continue”

        Select 1/64″ Flat End Mill

        Insert 1/64″ flat end mill

        Click “Continue”

        Allow homing again

        Verify tool position (usually just hit “Continue”). Note that the
“Continue” button takes a few seconds to become clickable.

        Verify safety zone (usually just hit “Locate”). Note that the “Locate”
button takes a few seconds to become clickable.

        In “Parts to Cut”, make sure that ONLY TRACES is selected

        Click “Start Cutting”, and then click “Cut!”

        When instructed, change the tool to the 1/32″ flat end mill and again
home the machine and locate the toolbit. Repeat for the 1/16″ end mill

        When the milling stops, it is time to flip the board and mill the
bottom. Note that the program doesn’t tell you this, it just stops.

        Move the platform to the front of the machine (Click “Loading” in
“Move to Position”) and remove your board. There is a thin spatula that can be
used to help unstick your board.

        Remove the tape from the bottom of your board

        Add tape to the other side of the board

        Stick your board to the Othermill taking great care:

            Flip it in the right direction

            Align your PCB against the forward RIGHT corner of the bracket

        Select the other side (“Side” button just below “Setup”)

        Allow homing again

        Verify tool position (usually just hit “Continue”)

        Verify safety zone (usually just hit “Continue”)

        In “Parts to Cut”, make sure all three (Traces, Holes, and Outlines)
are selected

        Click “Start Cutting”

        When instructed, change the tool to the 1/32″ flat end mill and again
home the machine and locate the toolbit. Repeat for the 1/16″ end mill

        When the milling stops, move the board to the front of the machine
(Click “Loading” in “Move to Position”) and remove your board. There is a thin
spatula that can be used to help unstick your board.


------------
1. Click “Loading” (in “Move to Position”)

1. Insert single sided PCB stock. Verify with a monitor that you have aligned
the PCB  to the correct corner of the bracket.
