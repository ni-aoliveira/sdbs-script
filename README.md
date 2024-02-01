# sdbs-script - SDBS status/restart process script

## Requirements:
You will need SSH access to all SDBS servers. If you don't have it, ask the hosting team to add your ssh key.

## Installation
* Just place the script under: `/usr/local/bin/`
* Give execution permissions: `chmod +x /usr/local/bin/sdbs`

## Examples of commands:
* Show the status of all processes on SDBS
```bash
sdbs stg status
```
* Show the status of a specific process
```
sdbs stg status sdbs-appserver-8095
```
* To restart all SDBS processes
```bash
sdbs stg restart all
```
* Restart a specific process
```bash
sdbs stg restart vfc:
```
```
sdbs stg restart sdbs-appserver-8095
```
## Commad skeleton:
```bash
sdbs <enviroment> <action> <process>
```
## List of environments accepted:
* dev (aka test)
* stg
* prod
## List of actions accepted:
* restart
* stop
* start
* status
## List of SDBS processes:
* collectd
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
* vfc:0                            
* vfc:1                           
* vfc:2
