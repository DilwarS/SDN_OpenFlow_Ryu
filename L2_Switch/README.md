# Layer 2 Switching Application

**Swicting Logic**

At layer 2 the switching will be based on MAC address of the hosts. So the flow will be  based on layer 2 match (source mac and destionation mac).

We will use ``` simple_swicth_13.py``` as base and modify to match the src and dst mac address. Save the file as ```L2_switch.py``` 


1.In a terminal run the ryu controller using the following command

``` ryu-manager L2_switch.py``` <br/>  

2. In a new terminal create a topology using the follwing command

```sudo mn --controller=remote,ip=127.0.0.1 --mac --topo=single,4```  

The above command will create a single toplogy four hosts.

3. In the sencond terminal (minine CLI) type ```pingall```  

4. To view the flow table of the swicth type the follwing command.  

```sudo ovs-ofctl dump-flows s1```
