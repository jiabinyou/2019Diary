//find element largest smaller than target, insert pos 在后面
//corner case: target前面没有元素，就插入在index = 0位置

class Solution {
    public int searchInsert(int[] nums, int target) {
        //sanity check
        if (nums == null || nums.length == 0) {
            return 0;
        }
        int left = 0;
        int right = nums.length - 1;
        while (left < right - 1) {
            int mid = left + (right - left) / 2;
            if (nums[mid] < target) {
                left = mid;
            } else {
                right = mid - 1;
            }
        }
        if (nums[right] < target) {
            return right + 1;
        } else if (nums[left] < target) {
            return left + 1;
        }
        return 0;
    }
}




