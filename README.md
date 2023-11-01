# sdbs-script - SDBS status/restart process script

## Requirements:
You will need ssh access to all SDBS servers. If you don't have it, ask hosting team to add your ssh key.

## Installation
* Just place the script under: `/usr/local/bin/`
* Give execution permissions: `chmod +x /usr/local/bin/sdbs`

## Examples of commands:
* Show the status of all processes on SDBS
```bash
sdbs test status
```
* To restart all SDBS processes
```bash
sdbs test restart all
```
* Restart a specific process
```bash
sdbs test restart vfc
```
## Commad skeleton:
```bash
sdbs <enviroment> <action> <process>
```
## List of enviroments accepted:
* test
* stage
* prod
## List of actions accepted:
* restart
* stop
* start
* status
## List of SDBS processes:
* masterdata                       
* sdbs-appserver-8091              
* sdbs-appserver-8091_http         
* sdbs-appserver-8091_mem          
* sdbs-appserver-8092              
* sdbs-appserver-8092_http         
* sdbs-appserver-8092_mem          
* sdbs-appserver-8093              
* sdbs-appserver-8093_http         
* sdbs-appserver-8093_mem          
* sdbs-appserver-8095              
* sdbs-appserver-8095_http         
* sdbs-appserver-8095_mem          
* vfc                              
* vfc-2                            
* vfc-3
