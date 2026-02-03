# Minecraft Server in WSL
For the sake of learning new things I thought how it will be to run a Minecraft server on my Raspberry Pi to play with my friends and in this way I can also showcase my Linux CLI understanding that I have gained so far. Running a Minecraft server on a Raspberry Pi it is not ideal becasue of hardware limitations, but in the end is a great project to learn Linux CLI basic commands.

# Server components
This project does not build a Minecraft server from scratch. Instead, it relies on well-established tools designed specifically for hosting Minecraft: Java Edition servers.

To run the server, the following components are used:

## PaperMC

The server application will be provided by PaperMC and can be found on https://papermc.io/ .

Paper is a high-performance Minecraft: Java Edition server implementation that focuses on:
-better optimization on low-performance devices
-a powerfull plugin API
-overall improved performance

## Startup Script
