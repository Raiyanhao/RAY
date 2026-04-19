class Solution {
    public int[] twoSum(int[] nums, int target) {
        // Line 3: Add 'int' before i
        for (int i = 0; i < nums.length; i++) { 
            // Line 4: 'int' is already there for j, so this is fine
            for (int j = i + 1; j < nums.length; j++) {
                if (nums[i] + nums[j] == target) {
                    return new int[] { i, j };
                }
            }
        }
        // This is a backup return in case no solution is found
        return new int[] {}; 
    }
}
