1. Largest element in an array...

import java.util.*;
class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the size of the array");
        int size = sc.nextInt();
        
        int arr[] = new int[size];
        System.out.println("Enter "+size+" elements");
        for(int i=0;i<size;i++)
        {
            arr[i] = sc.nextInt();
        }
        int largest = arr[0];
        for(int i=0;i<size-1;i++)
        {
            if(largest < arr[i])
            {
                largest = arr[i];
            }
        }
        System.out.println("Largest element is : "+largest);
    }
}

------------------------------------------------------------------------------------------

2. 2nd largest element...

import java.util.*;
class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the size of the array");
        int size = sc.nextInt();
        
        int arr[] = new int[size];
        System.out.println("Enter "+size+" elements");
        for(int i=0;i<size;i++)
        {
            arr[i] = sc.nextInt();
        }
        int largest = arr[0];
        int largest2 = arr[0];
        for(int i=1;i<size;i++)
        {
            if(largest < arr[i])
            {
                largest2 = largest;
                largest = arr[i];
            }
            else if(largest2>arr[i] && largest != arr[i]){
                largest2 = arr[i];
            }
        }
        System.out.println("Largest element is : "+largest);
        System.out.println("Second largest no. is : "+largest2);
    }
}

------------------------------------------------------------------------------------------

3. Check if Array Is Sorted and Rotated(LeetCode 1752)...

class Solution {
    public boolean check(int[] nums) {
        int dip = 0;
        int n = nums.length;
        for(int i=0;i<n;i++){
            if(nums[i]>nums[(i+1)%n])
            dip++;
        }
        //if(nums[nums.length-1]>nums[0])
        //dip++;

        if(dip <= 1)
        return true;
        
        else
        return false;
    }
}

------------------------------------------------------------------------------------------

4. Majority Element(LeetCode 169)...

class Solution {
    public int majorityElement(int[] nums) {
        int candidate = 0;
        int count = 0;

        for(int i=0; i<nums.length; i++)
        {
            if(count == 0){
                candidate = nums[i];
            }

            if(nums[i] == candidate){
                count++;
            }
            else
            count--;
        }
        return candidate;
    }
}

------------------------------------------------------------------------------------------

5. Two Sum(LeetCode 1)...

class Solution {
    public int[] twoSum(int[] nums, int target) {
        HashMap<Integer, Integer> map = new HashMap<>();
        int n = nums.length;
        for(int i=0;i<n;i++)
        {
            int left = target - nums[i];
            if(map.containsKey(left))
            {
                return new int[] {map.get(left),i};
            }
            map.put(nums[i],i);
        }
        return new int[] {};        
    }
}

------------------------------------------------------------------------------------------

6. Two Sum II - Input Array Is Sorted(LeetCode 167)...

class Solution {
    public int[] twoSum(int[] numbers, int target) {
        int i=0, j=numbers.length - 1;
        while(i<=j)
        {
            if(numbers[i] + numbers[j] == target)
            {
                return new int[] {i+1,j+1};
            }
            else if(numbers[i] + numbers[j] < target)
            {
                i++;
            }
            else j--;
        }
        return new int[] {};
    }
}

------------------------------------------------------------------------------------------

7. Subarray Sum Equals K(LeetCode 560)...

class Solution {
    public int subarraySum(int[] nums, int k) {
        HashMap <Integer, Integer> map = new HashMap<>();

        map.put(0,1);

        int prefixSum = 0;
        int count = 0;

        for(int i=0; i<nums.length; i++)
        {
            prefixSum += nums[i];
            count += map.getOrDefault(prefixSum - k , 0);
            map.put(prefixSum, map.getOrDefault(prefixSum,0)+1);
        }
        return count;
    }
}

------------------------------------------------------------------------------------------
