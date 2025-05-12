## 📘 Problem Statement

You are given two integer arrays `nums1` and `nums2`, sorted in **non-decreasing** order, and two integers `m` and `n` representing the number of elements in `nums1` and `nums2` respectively.

- `nums1` has a length of `m + n`, where the first `m` elements denote the elements to be merged, and the last `n` elements are set to `0` and should be ignored.
- Merge `nums2` into `nums1` as one sorted array in-place.

---

## 🧠 Approach

- Start merging from the end to avoid overwriting useful data.
- Use three pointers:
  - `k`: points to the end of the final merged array.
  - `l`: last element of the meaningful part in `nums1`.
  - `r`: last element in `nums2`.
- Compare values from the end and place the larger one at the end of `nums1`.

## ⏱ Time and Space Complexity
Time Complexity: O(m + n)

Space Complexity: O(1) – In-place merge
