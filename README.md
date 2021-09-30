# House-Robber

<!--
Note - Any content mention below in `<!-- ->` blocks are just comments
to help you fill-up the issue. It won't be visible in the actual issue after
you click on submit.
-->










#### Code you used for Submit/Run operation


```
// House Robber
class Solution {
    public int rob(int[] nums) {
        
        int n = nums.length;
        
        if(n==0){
            return 0;
        }
        if(n==1){
            return nums[0];
        }
        int[] dp = new int[n];
        dp[0] = nums[0];
        dp[1] = Math.max(nums[0],nums[1]);
        for(int i = 2;i<n ; i++)
        {
            dp[i] = Math.max(dp[i-1],nums[i]+dp[i-2]);
        }
        return dp[n-1];
    }
}
```

#### Language used for code
java 


#### Expected behavior
<!-- A clear and concise description of what you expected to happen in
contrast with what actually happened. -->
this question took my half an hour but the logic that i try to push in this code is having some plagiarism just because i take help of resources to complete this problem :)



#### Screenshots


![House-Robber](https://user-images.githubusercontent.com/53940939/135485819-46f3490d-b478-46c8-802d-89e01a8e7aa3.png)




Thankyou :)
