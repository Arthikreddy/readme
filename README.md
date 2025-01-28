# readme
4x4 Bit Approximate Multiplier This repository presents an approximation technique:

Approximation Techniques:

HALF ADDER:



![Screenshot 2025-01-28 222348](https://github.com/user-attachments/assets/f746dfbd-ca14-414d-b397-8ae2999a5a2d)


sum = a|b

carry = a&b

 By replacing xor with or gate power consumption can be reduced .As a result 1 out 0f 4 cases has an error in sum

 
 
 
 FULL ADDER:


 
 ![Screenshot 2025-01-28 222410](https://github.com/user-attachments/assets/c0f68717-7072-4a3b-ba20-59dbff0ab083)



in case of full addder :
 sum = a

  carry = b

As a result 4 out of 8 cases has errors 4 in sum and 2 in carry


COMPRESSOR :
4:2 Compressor Truth Table
Truth Table:

| A | B | C | D | Exact Sum | Exact Carry | Approx Sum | Approx Carry | E |
|---|---|---|---|-----------|-------------|------------|--------------|---|
| 0 | 0 | 0 | 0 |     0     |      0      |     0      |      0       | 0 |
| 0 | 0 | 0 | 1 |     1     |      0      |     1      |      0       | 0 |
| 0 | 0 | 1 | 0 |     1     |      0      |     1      |      0       | 0 |
| 0 | 0 | 1 | 1 |     0     |      1      |     1      |      1       | 1 |
| 0 | 1 | 0 | 0 |     1     |      0      |     1      |      0       | 0 |
| 0 | 1 | 0 | 1 |     0     |      1      |     1      |      1       | 1 |
| 0 | 1 | 1 | 0 |     0     |      1      |     1      |      1       | 1 |
| 0 | 1 | 1 | 1 |     1     |      1      |     1      |      1       | 0 |
| 1 | 0 | 0 | 0 |     1     |      0      |     1      |      0       | 0 |
| 1 | 0 | 0 | 1 |     0     |      1      |     1      |      1       | 1 |
| 1 | 0 | 1 | 0 |     0     |      1      |     1      |      1       | 1 |
| 1 | 0 | 1 | 1 |     1     |      1      |     1      |      1       | 0 |
| 1 | 1 | 0 | 0 |     0     |      1      |     0      |      1       | 1 |
| 1 | 1 | 0 | 1 |     1     |      1      |     1      |      1       | 0 |
| 1 | 1 | 1 | 0 |     1     |      1      |     1      |      1       | 0 |
| 1 | 1 | 1 | 1 |     0     |      1      |     0      |      1       | 1 |



Total errors in sum = 7

Total errors in carry = 11

compressor which is being is a 4:2 compressor with 4 inputs and 2 outputs as shown below:





![Screenshot 2025-01-28 222459](https://github.com/user-attachments/assets/bef48fcf-ccde-4528-86a5-0970641e1491)


sum=((a^b))|((c^d));
caryy=  (a&b)|(c&d);

Partial Product Transformation
The approximation involves the transformation of partial product terms am,n and an,m ( am,n = a[m]×b[n] ) into propagate and generate terms:

p a m,n = a m,n+ a n,m

g a m,n = a m,n ⋅ a n,m

No change in a a m,m terms

FINAL SUMMATION



![WhatsApp Image 2025-01-28 at 23 26 03_e7cf076d](https://github.com/user-attachments/assets/74fb67a7-4130-43da-ae57-4c0bce33f4c4)


BLOCK DIAGRAM:



![Screenshot 2025-01-28 221457](https://github.com/user-attachments/assets/83b22856-dc73-4e7a-bd39-2dc6209974a1)




RESULTS:
MEAN RELATIVE ERROR:Around 10.2%


![Screenshot 2025-01-28 221211](https://github.com/user-attachments/assets/58efddf5-36bc-4aee-8c84-3cd7b78799e7)



LUT UTILISATION:8


![Screenshot 2025-01-28 221624](https://github.com/user-attachments/assets/80b1810d-eea3-4d8c-be8f-e1cc7b547967)




POWER USAGE : 2.8W
LOGIC POWER : 28mW

![Screenshot 2025-01-28 221034 - Copy](https://github.com/user-attachments/assets/198fc24a-83bb-45fe-bc39-4d77a9544691)











