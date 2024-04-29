# patterns
the following has some patterns to practice.

### pattern 1.
```
    *    
   ***   
  *****  
 ******* 
*********


#include <iostream>
using namespace std;
int main() {
    int i,j,n;
    cin>>n;
    for(i=1;i<=n;i++){
        for(j=1;j<n-i+1;j++){
            cout<<' ';
        }
        for(j=1;j<2*i;j++){
            cout<<'*';
        }
        for(j=1;j<n-i+1;j++){
            cout<<' ';
        }
        cout << '\n';
    }
    return 0;
}
```

### pattern 2
```
 *** 
   ***   
     ***     
       ***       
         ***         


#include <iostream>
using namespace std;
int main() {
    int i,j,n;
    cin>>n;
    for(i=1;i<=n;i++){
        for(j=1;j<2*i;j++){
            cout<<' ';
        }
        for(j=1;j<n-1;j++){
            cout<<'*';
        }
        for(j=1;j<2*i;j++){
            cout<<' ';
        }
        cout << '\n';
    }
    return 0;
}
```
### pattern 3
```
 ******* 
  *****  
   ***   
    *    
          

#include <iostream>
using namespace std;
int main() {
    int i,j,n;
    cin>>n;
    for(i=1;i<=n;i++){
        for(j=0;j<i;j++){
            cout<<' ';
        }
        for(j=0;j< 2* n - (2*i+1);j++){
            cout<<'*';
        }
        for(j=0;j<i;j++){
            cout<<' ';
        }
        cout << '\n';
    }
    return 0;
}
```

### pattern 4

```
     *
    ***
   ***** 
  *******
 *********
***********  
***********
 *********
  *******
   ***** 
    ***    
     *


#include <iostream>
using namespace std;
int main() {
    int i,j,n;
    cin>>n;
    for(i=1;i<=n;i++){
        for(j=1;j<n-i+1;j++){
            cout<<' ';
        }
        for(j=1;j<2*i;j++){
            cout<<'*';
        }
        for(j=1;j<n-i+1;j++){
            cout<<' ';
        }
        cout << '\n';
    }
    for(i=0;i<n;i++){
        for(j=0;j<i;j++){
            cout<<' ';
        }
        for(j=0;j<2*n-((i*2)+1);j++){
            cout<<'*';
        }
        for(j=0;j<i;j++){
            cout<<' ';
        }
        cout<<'\n';
    }
    return 0;
}



```

### pattern 5

```
*
**
***
****
***
**
*



#include <iostream>
using namespace std;
int main() {
    int i,j,n;
    cin>>n;
    for(i=1;i<=2*n-1;i++){
        int stars = i ;
        if(i>n) stars= 2*n-i;
        for(j=1;j<stars;j++){
            cout<<'*';
        }
        
        cout << '\n';
    }
    return 0;
}

```

### pattern 6
```
1
01
101
0101
10101

#include <iostream>
using namespace std;
int main() {
    int i,j,n;
    cin>>n;
    int start =1;
    for(i=0;i<n;i++){
        if(i % 2 ==0)start=1;
        else start=0;
        for(j=0;j<=i;j++){
            cout<<start;
            start=1 - start;
        }
    cout<<'\n';

    }
    return 0;
}
```
### pattern 7
```
1        1
12      21
123    321
1234  4321

#include <iostream>
using namespace std;
int main() {
    int i,j,n;
    cin>>n;
    int space =2*(n-1);
    for(i=1;i<n;i++){
        for(j=1;j<=i;j++){
          cout<<j;
        }
        for(j=0;j<space;j++){
          cout<<' ';  
        }
        for(j=i;j>=1;j--){
          cout<<j;
        }
        cout<<'\n';
        space -= 2;
    }
    return 0;
}
```
