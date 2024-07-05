# Space Engineers Enhanced Hinge and Wheel Control
 Description of the Script  This script controls a hinge and wheels (suspension) in a Space Engineers grid based on the player's input from a control seat. It allows the player to move the hinge left or right using the "A" and "D" keys, move the wheels forward or backward using the "W" and "S" keys, and activate the handbrake using the "P" key.

Script Usage

1. Set Up Blocks:
- Name your hinge block to match `hingeName`.
- Name your wheel blocks to include `wheelGroupName`.
- Ensure your control seat is named `"maincontrol"` or adjust the script accordingly

2. Load the Script:
- Open the Programmable Block in your grid.
- Copy and paste the script into the Programmable Block's editor.

3. Compile and Run:
- Click "Check Code" to compile the script.
- Click "Remember & Exit" to save and exit.
- Set the Programmable Block to run with the desired update frequency (default is 10 ticks).

Here is a user-friendly description of the script, explaining its functionality and the configurable parameters:

Description of the Script

This script controls a hinge and wheels (suspension) in a Space Engineers grid based on the player's input from a control seat. It allows the player to move the hinge left or right using the "A" and "D" keys, move the wheels forward or backward using the "W" and "S" keys, and activate the handbrake using the "P" key.

Functionality

1. Hinge Control:
- A" Key: Moves the hinge to the left.
- D" Key: Moves the hinge to the right.
- No Key Pressed: Stops the hinge.

2. Wheel Control:
- "W" Key: Moves the wheels forward.
- "S" Key: Moves the wheels backward.
- No Key Pressed: Stops the wheels.

3. Handbrake:
- "P" Key: Activates the handbrake, stopping the wheels and preventing movement.

Configuration Parameters

Users can customize the script to fit their specific setup by changing the following parameters:

1. Hinge Name: The name of the hinge block in your grid.

string hingeName = "Hinge1";

Replace `"Hinge1"` with the custom name of your hinge block.

2. Wheel Group Name: A part of the custom name of all the wheels (suspensions) in your grid.

string wheelGroupName = "Wheel2";

Replace `"Wheel"` with a part of the custom name of your wheel blocks.

3. Control Seat Name: The name of the control seat in your grid (default is `"maincontrol"`).

IMyShipController controller = GridTerminalSystem.GetBlockWithName("ControlSeat") as IMyShipController;

Replace `"ControlSeat"` with the custom name of your control seat block if different.

4. Hinge Speed: The speed at which the hinge moves when the "A" or "D" keys are pressed.

float hingeSpeed = 5.0f;

Adjust the value of `hingeSpeed` to control how fast the hinge moves.

5. Wheel Speed: The speed at which the wheels move when the "W" or "S" keys are pressed.

float wheelSpeed = 10.0f;

Adjust the value of `wheelSpeed` to control how fast the wheels move.
