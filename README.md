# Brainmatters AI 


An AI written in NodeJS (+brain.js) that remote-controls execution of an emulator using 'nodegrpc'.

For the first iteration, the emulator will be 'RustBoyAdvance' using the rustnodegrpc package to receive JSONRPC commands. [-> Emulator source code](https://github.com/brainmatters/rustboyadvance-ng)


## Getting Started 

1. Install dependencies with 
` yarn install `

2. Boot the rust gba emulator [-> Emulator source code](https://github.com/brainmatters/rustboyadvance-ng)

3. Run the server with 
` yarn server `




## JSONRPC endpoints
###  The endpoints on the Rust-based GBA emulator  


sendControllerEvent(evt): sends a controller event like A, B, up, down, right, left 

readMemory(slot,length): reads the emulation RAM memory location at the specified slot and length   



setMemory(slot, newData): sets the RAM memory at the defined location to newData, hacking the RAM emulation state   [not rly necessary]