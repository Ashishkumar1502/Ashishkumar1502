- š Hi, Iām @Ashishkumar1502
- š Iām interested in ...
- š± Iām currently learning ...
- šļø Iām looking to collaborate on ...
- š« How to reach me ...

<!---
Ashishkumar1502/Ashishkumar1502 is a āØ special āØ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

#include <bits/stdc++.h>

using namespace std;

const int MAX_CHAR = 26;

bool arePermutation(string A, string B)

{

    // your code goes here

    int countA[MAX_CHAR] = {0};

int countB[MAX_CHAR] = {0};

    int l1 = A.length(), l2 = B.length();

   

    for(int i=0; i<l1; i++)

        countA[A[i]-'a']++;

    for(int i=0; i<l2;i++)

        countB[B[i]-'a']++;

       

       

       for (int i=0 ;i <26;i++)

           if ((countA[i] >1 && countB[i] == 0))

           return false;

    return  true;

}


