# RemoveIntances
#array nums and a value val, remove all instances of that value in-place and return the new length.

import java.util.Arrays;
class Solution {
     public int removeElement(int[] nums, int val) {
        int result = nums.length;
        for(int i=0;i<result;i++){
            if(nums[i]==val){
                for(int j=i;j<result-1;j++){
                    nums[j]=nums[j+1];
                }
                result--;
                i--;
            }
        }
        return result;
    }
}
