# Remove Linked List Elements

- Topic: Linked List
- Pattern: sentinel-node
- Submitted from: Leetcore
- Submitted at: 2026-07-02T05:27:50.579Z

## Solution

#include <iostream>
using namespace std;
int main()
{
  int n;
  cin>>n;
  int arr[n];
  for(int i = 0; i < n; i++)
  {
    cin>>arr[i];
  }
  int k;
  cin>>k;
  cout<<"[";
  for(int i = 0; i < n; i++)
  {
    if(arr[i] != k) cout<<arr[i]<<", ";
  }
  cout<<"]";
}
