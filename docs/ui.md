# The User Interface
This section will provide you with an overview of the user interface to assist your navigation on the various BCS screens.

## Help Links
By default, every section on the BCS UI has a ![question mark](img/ui/question-mark.png) next to it which contains a link to the relevant section in the manual.  This feature can be toggled on and off using the Toggle Help link at the bottom of every page.

![toggle help](img/ui/toggle-help.png)

## Process Bar

The Process Bar appears on the left hand side of all pages in the BCS interface so you can always see which processes are currently running and provides access to the All Stop button. 

![process bar](img/ui/process-bar.png) 

Processes can be started or stopped by clicking the process in the process bar.  The All Stop button will stop all processes and turn off all outputs that are currently on even if they are not being controlled by a process. Multiple processes can run at the same time. The names of the processes can also be customized on the [Process Editor](process_editor.md) page. A process is simply of set of rules or steps that can control various outputs (such as pumps, burners or valves) based on inputs like temperature probes, timers, or the state of other digital inputs.

The '<' link below the process bar can be used to hide the process bar if it is not needed.  This can help with space restrictions on smaller screens.

## Main Control UI

The Main Control UI is the main interface for using the BCS. It displays the current temperature for all enabled temperature probes, information on running processes, and the current status of all enabled outputs and inputs.

![control ui with process](img/ui/control-ui-process.png)
*Above: Main Control UI with a running processes*

At the top of the Control UI is the navigation bar. Each of the individual pages of the BCS interface can be accessed from the navigation bar. Each of the pages on the navigation bar has its own corresponding page in this user guide.
![navigation bar](img/ui/nav-bar.png)


### Temperatures

The BCS offers 3 options for viewing the current temperatures.

Style         | 
------------- | ------------------------------------
Dial Style    | ![Dial Style](img/ui/dial.png)
LED Style     | ![LED Style](img/ui/LED.png)
Compact Style | ![Compact Style](img/ui/compact.png)

*The compact style is great on mobile devices!*

### Processes

Running processes will be shown directly on the Control UI.  Processes can also be set up with an option so they are always displayed.

![running process](img/ui/process-control.png)

The process can be paused or resumed using the button in the upper right hand corner.

The state can be changed directly by clicking on the desired state in the process section.

Clicking the name of the process will stop (or start) the process.



### Outputs
Displays the current state of the outputs.

![outputs](img/ui/outputs.png)

Outputs can be manually controlled by clicking on them in the Control UI, but any running processes or ladder logic will take precedence.

### Inputs
Displays the current state of the inputs.

![inputs](img/ui/inputs.png)
Digital inputs are controlled by external push button switches, toggle switches or, devices like float switches.  These are generally used for triggering state changes within a process.