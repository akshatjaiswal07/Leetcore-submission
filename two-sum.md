# Two Sum

- Topic: Array
- Pattern: hash-map
- Submitted from: Leetcore
- Submitted at: 2026-07-01T16:20:38.876Z

## Solution

/**
 * @param {number[]} nums
 * @param {number} target
 * @return {number[]}
 */
function twoSum(nums, target) {
    const numMap = new Map();
    
    for (let i = 0; i < nums.length; i++) {
        const complement = target - nums[i];
        
        if (numMap.has(complement)) {
            return [numMap.get(complement), i];
        }
        
        numMap.set(nums[i], i);
    }
    
    return [];
}
