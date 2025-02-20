# experiment-no.-4-22BCS_IOT-701B
https://leetcode.com/problems/longest-nice-substring/description/
https://leetcode.com/problems/maximum-subarray/description/
Experiment no. 4
```bash
class Solution {
    public int maxSubArray(int[] nums) {
        int maxSum = nums[0];  // Initialize maxSum with the first element
        int currentSum = nums[0];  // Initialize current running sum

        for (int i = 1; i < nums.length; i++) {
            // Either add the current element to the previous sum or start a new subarray
            currentSum = Math.max(nums[i], currentSum + nums[i]);
            // Update the maximum sum found so far
            maxSum = Math.max(maxSum, currentSum);
        }
        return maxSum;
    }
}
![Screenshot 2025-02-20 110354](https://github.com/user-attachments/assets/874fdd16-5bfc-4325-95b0-062d32ac67fd)
```
