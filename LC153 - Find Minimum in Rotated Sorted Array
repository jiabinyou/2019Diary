/*
input: no dup
结果一定存在

mid和right相比
array[mid] < array[right] -->往左,mid可能是res
		else                                --> 往右，mid不可能是结果
*/
class Solution {
    public int findMin(int[] nums) {
        int left = 0;
        int right = nums.length - 1;
        while (left < right) {
            int mid = left + (right - left) / 2;
            if (nums[mid] < nums[right]) {
                right = mid;
            } else {
                left = mid + 1;
            }
        }
        return nums[left];  
    }
}
