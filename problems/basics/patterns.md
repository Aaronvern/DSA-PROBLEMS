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
