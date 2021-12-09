
# Question description:

> Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.
> You may assume that each input would have exactly one solution, and you may not use the same element twice.
> You can return the answer in any order.

Case1
```
Input: nums = [2,7,11,15], target = 9
Output: [0,1]
Output: Because nums[0] + nums[1] == 9, we return [0, 1].
```

Constraints:

>2 <= nums.length <= 104
>-109 <= nums[i] <= 109
>-109 <= target <= 109
>Only one valid answer exists.

Code with C ++:
> Method 1: Enumerate
> the time complexity will be O(n^2), space complexity will be O(1)
```
class Solution {
    public:
    vector<int> twoSum(vector<int>& nums, int target) {
        int n = nums.size();
        for ( int i = 0; i < n, i++ ){
            for ( int j = i + 1; j < n; j++){
                if ( nums[i] + nums[j] == target ){
                    return {i, j};
                }
            }
        }
        return;
    }
};
```

> Method 2: Hash map

```





