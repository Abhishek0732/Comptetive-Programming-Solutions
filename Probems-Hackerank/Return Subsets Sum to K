import java.util.*;
public class Solution 
{
    public static ArrayList<ArrayList<Integer>> findSubsetsThatSumToK(ArrayList
    <Integer> arr, int n, int k) 
	{
        // Write your code here.
        ArrayList<ArrayList<Integer>> ans = new ArrayList<>();

        solve(0,0,n,arr,k,ans,new ArrayList<>());
        return ans;
    }
    public static void solve(int ind, int sum,int n,ArrayList<Integer> arr,
    int k, ArrayList<ArrayList<Integer>> ans,ArrayList<Integer> ds){
        if(ind==n){
            if(sum==k){
                ans.add(new ArrayList<>(ds));
            }
            return;
        }
        ds.add(arr.get(ind));
        solve(ind+1,sum+arr.get(ind),n,arr,k,ans,ds);
        ds.remove(ds.size()-1);
        solve(ind+1,sum,n,arr,k,ans,ds);
    }
}
