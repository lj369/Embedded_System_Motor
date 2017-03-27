# Embedded_System_Motor

This code can be type in the following command

R and 3 digit number, decimal point and number after it which specify the number of rotation of motor

V and 3 digit number which specify the speed of motor

For tone, all commands are also in capital letters where the note can be followed by # or ^ and must contains number which specify the length of playing

Our commands follow exactly

T([A-G][#\^]?[1-8]){1,16}

and

(R-?\d{1,3}(\.\d{1,2})?)?(V\d{1,3}(\.\d{1,3})?)?

P.S. There are 2/4 states difference between rotor state read from I1I2I3 and Motor inductor state. Setting leads may be required. setting of leads are inside input_callback_ex fumction, change two rotation direction values according to your motor state difference, otherwise it may not even rotate.  
