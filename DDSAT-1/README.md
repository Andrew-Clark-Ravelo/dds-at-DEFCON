# DDSAT-1
DDSat-1 focuses on showing the problems with how many of the control messages for satellites are either naturally unencrypted, or kick to an unencrypted mode should the satellite not be able to communicate with the ground station.  

To do this remotely, a chatbot will post Manchester encoded data in the chat as if it had just passed through a BPSK filter.  Effectively, we are skipping the RF part of the AMSAT standard and focusing on the data representation fields.  Users will then have to decode and analyze the data to begin parsing out fields and identifying which messages are from the ground station and which are from the satellite.  After they have identified the message format, they can begin attacking the different payload and control systems via RF.  This will allow them to do things like change telemetry, control a camera, and change what the satellite is broadcasting.  However, because they are not able to remove the valid ground station, they’ll have to plan out their attacks knowing that the ground station will attempt to correct any abnormal behaviors.  