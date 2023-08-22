# Millumin x Subtext
Instructions for how to use Subtext with Brightsign with an accompanying example

## Setup
* **Protocol**: OSC+Freerun
* **Software**: Millumin 4.16.f

## Instructions
1. Add new Data track ![add data](assets/add_data.png)
2. Add media to the dashboard
3. Select the data track and open the device management panel ![open panel](assets/open_panel.png)
4. Add an OSC server if necessary and input the node's ip address and port. Ensure it is enabled ![add server]
   (assets/add_server.png)
5. Close the device management panel
6. On the data track, ensure the method is set to "command"
7. Add a string to the column and enter "/start_freerun 1" ![add cue](assets/add_cue.png)

### N.B.
Looping videos will not re-trigger data track commands. You must set up a pair of auto-go commands, one to continue 
to the next column when the media is complete, and one to relaunch the first column. ![auto go](assets/auto_go.png)

## Reference
https://help.millumin.com/docs/connect/devices/