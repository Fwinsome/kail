# kail
#include<bits/stdc++.h>
using namespace std;
	long long l,n,m,a[1000001],b[1000001];
int main(){
	cin>>l>>n>>m;
	for(int i=1;i<=n;i++){
		cin>>a[i];
	}
	a[0]=0;
	a[n+1]=l;
	for(int i=1;i<=n+1;i++){
		b[i]=a[i]-a[i-1];
	}
	int l=0,o=1,fa=0;
	int r=l;
	int mid;
	while(true){
		mid=l+(r-l)/2;
		for(int i=1;i<=n+1;i++){
				if(mid>b[i]){
					fa++;
					b[i]=b[i]+b[i-1];
				}
		}
		if(fa>m){
			fa=0;
			mid=mid/2;
			continue;
		}
		if(fa=m){
			cout<<mid;
			return 0;
		}
	}
	return 0;
} 
