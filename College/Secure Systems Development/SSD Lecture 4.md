* [[SSD Lecture 1]]
* [[Stack Smash Attack]]
* Multiple protections exist to prevent stack attacks on modern OS
* **Stack protector** -> random number before return address -> if [[Stack Smash Attack]] occurs, it will overwrite this random number, if the integrity of this is compromised, it will abort the process
* 