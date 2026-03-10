class Solution {
    static ArrayList<Integer> subarraySum(int[] arr, int target) {
        int sum = 0;
        int j = 0;
        ArrayList<Integer> ans = new ArrayList<>();
        for(int i = 0; i < arr.length; i++) {
            sum = sum + arr[i];
            while(sum > target && j <= i) {
                sum = sum - arr[j];
                j++;
            }

            if(sum == target) {
                ans.add(j + 1);
                ans.add(i + 1);
                return ans;
            }
        }

        ans.add(-1);
        return ans;
    }
}
