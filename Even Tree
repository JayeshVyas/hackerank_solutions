#include<bits/stdc++.h>
using namespace std;
int main()
{
    int V,E;
    cin>>V>>E;
    int array[E][2];
    for(int i=0;i<E;i++)
    {
         cin>>array[i][0]>>array[i][1];
    }
    int count[V+1];
    for(int j=0;j<=V;j++)
    {
        count[j]=1;
    }
    for(int k=0;k<E;k++)
    {
        count[array[k][1]]=0;
    }

  int c=0,l;
    for(int i=V;i>=0;i--)
    {
        if(count[i]==0)
        {
            for(int k=0;k<E;k++)
            {
                if(array[k][1]== i)
                {   l=array[k][0];
                    if(count[l]%2 != 0)
                    {
                    c=c+count[l];
                    }
                 }
            }
            count[i]=c+1;
        }
        c=0;
    }
    int t=0;
    for(int i=0;i<=V;i++)
        {
            if(count[i]%2 == 0)
            {
                t=t+1;
            }
        }

        cout<<(t-1)<<endl;
    return 0;
}
