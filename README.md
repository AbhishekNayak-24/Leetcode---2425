# Leetcode---2425
Bitwise XOR Of All Pairings
// code in java
public class Solution {
    public int xorAllNums(int[] nums1, int[] nums2) {
        int xor1 = 0, xor2 = 0;
        for (int num : nums1) xor1 ^= num;
        for (int num : nums2) xor2 ^= num;
        return (nums1.length % 2) * xor2 ^ (nums2.length % 2) * xor1;
    }
}
