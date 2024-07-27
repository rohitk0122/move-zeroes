# move-zeroes
class Solution {
    public void moveZeroes(int[] nums) {
       int nonZeroIndex = 0;  // Keeps track of the index to place the non-zero element
        
        // Traverse through the array
        for (int i = 0; i < nums.length; i++) {
            if (nums[i] != 0) {
                // Swap the elements
                int temp = nums[nonZeroIndex];
                nums[nonZeroIndex] = nums[i];
                nums[i] = temp;
                nonZeroIndex++;
            }
        } 
    }
}
