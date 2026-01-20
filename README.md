🔊 TITAN AUDIO: The "It Just Works" Protocol
Welcome to Titan Audio. This is what happens when you get tired of "professional" audio software having more lag than a dial-up connection in a middle-of-the-ocean thunderstorm. It’s a raw, 32-bit float, UDP-shoveling beast that turns your local network into a virtual copper wire.
🧪 What is this?
Titan is a point-to-point audio streamer. It captures your Mic and your Virtual Cable (Brave, Discord, or any system loopback), mixes them into a single high-fidelity soup, and fires them across your Local Area Network (LAN).
No compression. No BS. No "Searching for Peers." Just raw voltage in digital form moving at the speed of your Ethernet cable.
🏠 The "Local Only" Disclaimer (For the Moment)
For the moment, this is a LAN-only party.
• 
Will it work in your house? Yes, and it'll be faster than a greased pig.
• 
Will it work over the Internet? Not unless you're a networking wizard who likes messing with Port Forwarding and NAT traversal.
• 
Why? Because the "Internet" is a mess of lost packets, and Titan doesn't have time for the Internet's feelings. It wants high-speed, low-latency local traffic only.
🛠 The "Tech Stuff" (For the Nerds)
• 
32-Bit Floating Point: Because 16-bit is for the 90s and we don't like digital clipping.
• 
Adaptive Master-Clocking: The Receiver actually listens to the Sender. If the Sender says "I'm 48kHz," the Receiver reconfigures its hardware to match. No more "Chipmunk Voice" or "Demon Slow-Mo."
• 
The Smooth-Glide Jitter Buffer: Custom sequence-snapping logic. If your WiFi hiccups and drops a packet, the engine just glides to the next one instead of stuttering like a bad dubstep track.
• 
UDP Direct-Pipe: We bypassed the TCP "handshake" nonsense. We don't care if a packet gets lost; we're already playing the next one.
 
🚀 How to Not Break It (Setup)
1. 
The Receiver: Run Receiver.exe on the computer that wants to hear the audio. It will sit there waiting for a "Sync" packet.
2. 
The Sender: Run Sender.exe on the computer making the noise.
3. 
The Choice: Select your Microphone index and your Virtual Cable index from the console list.
4. 
The Magic: The moment the Sender starts, the Receiver will snap to the correct sample rate and start playing.
Pro-Tip: Make sure both computers are on the same router/subnet. If your Windows Firewall asks "Can this talk to the network?", say YES.
 
⚠️ About the Included Files
I included the Program Database (.pdb) files in the repository.
• 
What they are: Debugging symbols.
• 
Why they are here: To help you (or me) find exactly where the code exploded if it hits a snag.
• 
Can you delete them? Yes. If you want a smaller folder, delete everything except the .exe and the .cpp files. The program doesn't need the PDBs to go fast.
 
📜 The Chronicles of Titan (Changelog)
Version
Status
The Struggle
v1.0
Proof of Concept
It made noise. It also crashed if you looked at it funny.
v4.2
The "Demon" Era
Audio worked, but everyone sounded like they were in a slow-motion horror movie (44.1k/48k mismatch).
v9.0
Legit Sync
Implemented GetMixFormat. The Sender now dictates the truth to the Receiver.
v10.5
The 3-Minute Death
Fixed a bug where audio would lag by 3 minutes after the buffer exploded. Added the "Safety Valve."
v11.2
Current Release
Added "Smooth-Glide" to kill the "Dubstep Wobble." Optimized for LAN-only stability.
Export to Sheets
Copy table
 
⚖️ License
MIT. Take it, break it, fix it, just don't blame me if you blast 32-bit float static at 100% volume and wake up the neighborhood.
