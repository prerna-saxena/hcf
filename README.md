# hcf



#include <iostream>

using namespace std;

int findhcf(int x, int y){
    int smallest=min(x,y);
    if(x%smallest==0&& y%smallest==0)
       return smallest;
       
       for(int i=smallest/2; i>=2; i--){
           if(x%i==0 && y%i==0)
             return i;
             
       }
       return 1;
       
    
}
