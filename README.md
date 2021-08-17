# Booth-Multiplier
Implemented Booth Multiplier using VHDL
A generic multiplier implemented using repeated additions is not efficient enough to be used in most applications.
Hence special multippliers are used which take lesser amount of delay. One of such multipiers is Booth Multiplier.

In this implementation of Booth Multiplier, two entities have been created namely Booth and alu_shift_and_add.
The booth entity depending upon the booth algorithm identifies whether to add, sub and by what amount- +1,-1,+2.
This information is sent to the alu_shift_an_add entity which if +1/-1 is required simply adds 1/-1. otherwise if 
+2 is required to be impleented it uses a barrely shifter to implement that.

By this we will get partial products. Then we just have to sum them up as done in the Booth entity.
