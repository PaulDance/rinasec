## Article notes, remarks, questions

 * II. B. Need clarification about EFCP instanciation on connection establishment.
   --> Probably nothing more than what it says.
 
 * III. B. Given that the amount of possible CEP ids, 2^16, is square root less
   than of possible ISNs, 2^32, then why would it be less prone to scan attacks
   through connection opening? What is the typical MPL? Even if it is a relatively
   short amount if time, wouldn't it be possible to launch multiple of such attacks
   in parallel to probably succeed every time and thus achieve connection opening
   after a few trials?
   --> The MPL should be set by the AP. To compare with TCP, how long is a SYN
       kept in memory before the correct SYN+ACK is answered?
 
 * III. D. Not very precise. Can't the service name be public? Why would using
   multiple DIFs be necessarily easier on the end system than with just one? If
   the attacker is already on a DIF that can reach the system with a sufficient
   amount of allocated resources, is it really a good protection mechanism? Even
   if there is an automatic connection ending mechanism through timers, wouldn't
   the attacker still be able to DoS the system using connection-opening attacks
   with frequent refreshes?
   --> See IPC authentication.
 
 * V. If an attacker was able to be authenticated once, couldn't they share the
   same connection details with multiple machines to create a sufficient flow of
   data messages towards the end system and thus achieve a DDoS attack?

   > no more consideration of security was present in the development of RINA
   > than in the development of the TCP/IP architecture.

   Really? Even with all the authentication, confidentiality, integrity and
   resilience considerations that are part of the initial design?
   --> Not very honest, sure.

