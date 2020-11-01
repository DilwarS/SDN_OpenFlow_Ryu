


# OpenFlow Switching Applications

# 1 Hub Application

# hub.py

When a data frame arrives at a port in hub, it is simply broadcast to every other port, without considering whether it is destined for a particular destination or not. ```hub.py``` is simply braodcast the packets out of every port without sending the packets to the controller.


how to run the hup.py application

In one terminal run the ryu controller using the follwing command

  ```ryu-manager hub.py```
  
In another terminal run the mininet
  
  ```sudo mn --controller=remote,ip=127.0.0.1 --mac --topo=single,4```
  


