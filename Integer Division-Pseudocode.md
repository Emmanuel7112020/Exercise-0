Firstly, an algorithm is expected to have the following properties.
•	Finiteness of number of steps
•	Definiteness of steps(specificity)
•	Input
•	Output, which is related to the inputs

1.	Pseudocode
Algorithm div
INPUT: An n element list_data
	The length_n_of_data
OUTPUT: The division_div_of a set of numbers.
Quotient=0
Remainder=0
For N=0 to n; y>0
Counter=counter + N
Quotient =data[N]/y
remainder =N-quotient*y
OD
If counter>0 THEN
	N=(quotient*y) + remainder
RETURN quotient
END

Algorithm
public class Division{
public static int div(int x, int y){
// z is the quotient and r is the remainder
 int z;
 int r;              
 int [ ] N={0,1,2,3,.....n};
 int a= N.length;
for(x<=N[a];y!=N[0];a--){
    z=x/y;
    r=x%y;
     }
 return z;
    }
}

2.	The above algorithm terminates because there is a definite number of steps as determined by the finite length of N and definiteness of range of numbers that can be assumed by N and y. In addition, the loop includes stepwise decrement for the length of the array. This approach guarantees that the algorithm terminates for all allowed values.
The values of x are from the highest number in the array to the lowest, while the values of y are any value in the array except 0.
3.	The algorithm could be altered by replacing “RETURN quotient (z)” with “RETURN remainder(r)”.

public class Division{
public static int div(int x, int y){
// z is the quotient and r is the remainder
 int z;
 int r;              
 int [ ] N={0,1,2,3,.....n};
 int a= N.length;
for(x<=N[a];y!=N[0];a--){
    z=x/y;
    r=x%y;
     }
 return r;
    }
}



4.	If the domain of the algorithm was extended to whole numbers, the algorithm would be as written below,
public class Division{
public static int div(int x, int y){
// z is the quotient and r is the remainder
 int z;
 int r;   
// it is assumed that N=Z =whole numbers, which could be either positive or negative           
 int [ ] N={-n,...-1,0,1,2,3,.....n};
 int a= N.length;
for(x<=N[a];y!=0;a--){
    z=x/y;
    r=x%y;
     }
 return z;
    }
}
