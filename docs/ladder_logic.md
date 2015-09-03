# Ladder Logic #

While programming processes can provide a robust method for programming complex interactions on the BCS, sometimes it is more efficient to use low level programming. That is what ladder logic provides. You do not have to use ladder logic, but if you do it supersedes any processes that have been configured. In addition, unlike processes, ladder logic is always running when the BCS is powered on.


## Ladder Logic

Ladder logic is based on Boolean functions such as AND and OR. Each rung has five slots. The first four slots are contacts and the last column is a coil. The coil slot is the result of the logic configured in the first four slots. Each slot must be filled with either a Process, Input, Output, Register, or Contact. The slots are connected to each other using Wires. Rungs are in groups of four. Rungs in the same group can be connected using wires. Rungs in different groups cannot be connected directly, but can be connected using Registers (explained below). When changes are made to the ladder logic, they are automatically saved and applied immediately.


### Wires

Wires are used to connect slots. In order for ladder logic to work, all the slots in a rung must be filled and all the slots must be connected using a wire. When a single rung is connected all the away across from left to right, the relationship between the slots is a logical AND. Slots can also connect via wires to slots above or below as long as they are in the same four rung group. When slots are connected vertically, the relationship between the slots is a logical OR. 

There are several different wire types to choose from to connect slots both horizontally and vertically. To add a wire between slots, simply drag and drop the desired wire from the right side menu to desired location on the ladder. To clear a previously applied wire connection, drag and drop the blank wire icon to the desired spot.

![wire icons](img/ladder_logic/wires.png)


### Contacts

Contacts are used to fill slots when you do not need a register, DIN, output, or process to fill that slot. Remember, every slot in the rung must be filled with one of these variables, so contacts are very useful. To add a contact to a slot, simply drag the contact to the desired slot. To clear the contact, drag the blank contact icon to the slot.

![contact icons](img/ladder_logic/contacts.png)


### Registers

Register are internal virtual switches on the BCS. Registers can be normally open (NO) or normally closed (NC). Since registers are virtual switches, their status can be used to control other register, outputs, and processes. Registers can also be used to extend ladder logic between rungs, even if they are in another rung group. There are sixteen available registers, numbered 0-15. For more information on how registers can be used, see the examples later in this section.

![register icons](img/ladder_logic/registers.png)


### Inputs

Inputs are the external discrete inputs (DINs) connected to the BCS. In ladder logic, each DIN can be either normally open (NO) or normally closed (NC). The dispostion of a DIN can control the status of registers, outputs, or processes. An input cannot be placed in the coil position. A common use of an input would be to use an external button or switch that in turn controls an output that will turn a pump on or off through ladder logic. For more information on how inputs can be used, see the examples later in this section.

![input icons](img/ladder_logic/dins.png)

### Outputs
An output can be placed in a contact position (columns 1-4) or a coil position (column 5). Each output is available as normally open (NO) and normally closed (NC). While outputs are normally thought of as coils, they can also be used as contacts. See the examples below for more information. If the output is placed in the coil position and all the conditions are met in the contacts, then the output will either be turned on (NO) or off (NC).

![output icons](img/ladder_logic/outputs.png)


### Processes

Like outputs, processes can also be placed in either contact or coil slots on the ladder. This behavior is useful is you want to use one process to start or stop another process. Processes can also be started or stopped using and input. Each process is available as running (NO) or stopped (NC).  For more information on how processes can be used, see the examples later in this section.

![process icons](img/ladder_logic/processes.png)


## Examples ##
Below are some common configuration examples using ladder logic. Use the examples below to help build out your ladder logic based on how you use your BCS. Remember, ladder logic takes precedence over any processes that are running. If you have a process running that has an output turned off, but that same output is turned on in ladder logic, then the output will be turned on.

### Example 1


### Example 2


### Example 3


### Example 4

