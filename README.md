# Experiment-2 
## **DC, Transient , AC analysis of Common Source Amplifier with Active load** <br>
 <p>The circuit consists of a PMOS and an NMOS transistor connected in a complementary configuration, operating at a supply voltage of 1.8V. The purpose of this design is to analyze its DC, transient, and AC responses to evaluate its frequency response.</p>

 ### <ins> Design Specifications </ins>
<table>
  <tr>
  <th> Parameters </th>
  <th> Description </th>
  </tr>
  <tr> 
  <td>Model</td>
    <td> CMOSN, CMOSP</td>
  </tr>
  <tr>
    <td>Supply Voltage</td>
    <td> 1.8V</td>
  </tr>
  <tr>
    <td> PMOS</td>
    <td> Acts as the pull up  network</td>
  </tr>
  <tr>
    <td> NMOS</td>
    <td> Acts as the pull down network</td>
  </tr>
  <tr>
    <td>V<sub>tp</sub></td>
    <td>-0.39V</td>
  </tr>
  <tr>
    <td>V<sub>tn</sub></td>
    <td>0.36V</td>
  </tr>
  <tr>
    <td> PMOS Length</td>
    <td> 180µm</td>
  </tr>
  <tr>
    <td> NMOS Length</td>
    <td> 180nm</td>
  </tr>
  <tr>
    <td> PMOS Width</td>
    <td> 0.209513mm</td>
  </tr>
  <tr>
    <td> NMOS Width</td>
    <td> 0.209µm</td>
  </tr>
  <tr>
    <td> 𝜇<sub>n</sub></td>
    <td> 273.809 m<sup>2</sup>/V</td>
  </tr>
  <tr>
    <td>𝜇<sub>p</sub></td>
    <td> 115.689 m<sup>2</sup>/V</td>
  </tr>
  <tr>
    <td> T<sub>oxn</sub>, T<sub>oxp</sub></td>
    <td> 4.1*10<sup>-9</sup>m</td>
  </tr>
  <tr>
    <td>𝜀<sub>ox</sub></td>
    <td> 3.45*10<sup>-11</sup> F/m</td>
  </tr>
</table> <br>

<ins> **Circuit Diagram** </ins> <br>

![Image](https://github.com/user-attachments/assets/2b65b9d3-ce13-47b6-a735-0a1275f93a65) <br>
The body terminal of both NMOS and PMOS is connect to drain terminal. <br><br>
To find the value of biased voltage: <br>
  We know that current flowing through the NMOS and PMOS is the equal; i.e I<sub>dn</sub> = I<sub>dp</sub> <br><br>
  <ins> Calculation: </ins> <br>
  <p> (1/2 * k<sub>n</sub> * (V<sub>gs</sub> - V<sub>tn</sub>)<sup>2</sup> ) = (1/2 *  k<sub>p</sub> * (V<sub>dd</sub> - V<sub>bias</sub> - |V<sub>tp</sub>|)<sup>2</sup> ) <br>
  C<sub>oxn</sub> =  C<sub>oxp</sub> = 3.45*10<sup>-11</sup> /  4.1*10<sup>-9</sup> = 8.41*10<sup>-3</sup> F/m <br>
    k<sub>n</sub> = 273.809 *  8.41*10<sup>-3</sup> = 2.303 A/V<sup>2</sup> <br>
    k<sub>p</sub> = 115.689 *  8.41*10<sup>-3</sup> = 0.973 A/V<sup>2</sup> <br>
  (0.5 * 2.303 * (0.209153µ / 180n) * (0.9 -0.366)<sup>2</sup> )= (0.5 * 0.973 * (0.209µ / 180n) * ( 1.8 - V<sub>dd</sub> - 0.39)<sup>2</sup> ) <br>
  0.373 = 0.54 * ( 1.8 - V<sub>dd</sub> - 0.39)<sup>2</sup> ) <br>
  $\sqrt{0.69}$; = 1.8 - 0.39 - V<sub>bias</sub> <br>
  0.83 = 1.41 - V<sub>bias</sub> <br>
  V<sub>bias</sub> = 0.58V 
</p> 

## <ins> **DC Analysis** </ins> <br><br>
<ins> **Circuit Diagram** </ins> <br>
![Image](https://github.com/user-attachments/assets/3308456d-6df6-4c78-ad20-195c6cf39a23) <br>
From the simulation : <br>
V<sub>out</sub> = 1.42V, I<sub>d</sub> = 9.4µA <br><br>
## <ins> **Transient Analysis** </ins> <br><br>
<ins> **Circuit Diagram** </ins> <br>
![Image](https://github.com/user-attachments/assets/04ca698e-838c-4d5b-af32-c963c0c2f589) <br>
<br>
## <ins> **AC Analysis** </ins> <br><br>
<ins> **Circuit Diagram** </ins> <br>
![Image](https://github.com/user-attachments/assets/99ed68fb-ddd6-4977-941c-c2daa355290a) <br>
