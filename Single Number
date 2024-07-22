class Solution {
    public int singleNumber(int[] nums) {
        int xorr = 0;
        for (int num : nums) {
            xorr ^= num;
        }
        return xorr;
    }
    public static void main(String[] args) {
        Solution solution = new Solution();
        int[] nums = {4, 1, 2, 1, 2};
        System.out.println(solution.singleNumber(nums)); 
    }
}
