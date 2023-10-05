#include <bits/stdc++.h> 
vector<int> findArraySum(vector<int>&a, int n, vector<int>&b, int m) {
	int sum{}, carry{};
	int i=n-1,j=m-1;
	vector<int> totalsum;
	while(i>=0 && j>=0)
	{
		sum=a.at(i)+b.at(j)+carry;
		carry=sum/10;
		sum=sum%10;
		totalsum.insert(totalsum.begin(),sum);
		i--;
		j--;
	}

	while(i>=0)
	{
		sum=a.at(i)+carry;
		carry=sum/10;
		sum=sum%10;
		totalsum.insert(totalsum.begin(),sum);
		i--;
	}

	while(j>=0)
	{
		sum=b.at(j)+carry;
		carry=sum/10;
		sum=sum%10;
		totalsum.insert(totalsum.begin(),sum);
		j--;
	}

	if(carry!=0)
	{
		totalsum.insert(totalsum.begin(),carry);
	}

	return totalsum;

}
