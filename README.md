# The Cheroz Algorithm: A Hybrid Sorting Approach

The **Cheroz Algorithm** is a hybrid sorting algorithm that combines the strengths of **Heap Sort** and **Insertion Sort** to deliver efficient performance across various data distributions and sizes. Designed as both an educational and exploratory tool, it leverages the adaptability of Insertion Sort for smaller or nearly sorted arrays and the robustness of Heap Sort for larger datasets.

---

## Features  

- **Adaptive Threshold**  
  Dynamically switches between Heap Sort and Insertion Sort based on input size and distribution.  

- **Enhanced Sorting**  
  Incorporates a modified version of Insertion Sort to efficiently handle partially sorted arrays.  

- **Versatile Performance**  
  Performs well on random, sorted, and reverse-sorted datasets.  

- **Scalable Design**  
  Handles arrays ranging from 100 to 1,000,000 elements with ease.  

---

## Methodology  

1. **Heap Sort Phase**  
   Creates an initial sorted structure for larger datasets using Heap Sort.  

2. **Insertion Sort Phase**  
   - Standard Insertion Sort for small, unsorted arrays.  
   - Enhanced Insertion Sort to identify and optimize sorted subsequences within larger arrays.  

3. **Threshold Switching**  
   A calculated threshold determines the transition point between Heap Sort and Insertion Sort.

---

### Pseudocode  

```text
procedure HYBRIDSORT(arr)
    n ← length of arr
    threshold ← DETERMINE_THRESHOLD(n)
    HEAPSORT(arr, 0, n - 1)
    if n ≤ threshold then
        INSERTION_SORT(arr, 0, n - 1)
    else
        ENHANCED_INSERTION_SORT(arr, 0, n - 1)
    end if
end procedure
```

---

## Usage  

### Requirements  

- A programming environment supporting **C++** or **Python** for algorithm implementation.  
- Test datasets (random, sorted, reverse-sorted arrays).  

### Steps to Implement  

1. Define the hybrid sorting function using the pseudocode provided.  
2. Generate datasets of varying sizes and distributions.  
3. Run the Cheroz Algorithm and compare its performance against standalone Heap Sort and Insertion Sort.

---

## Results and Observations  

- **Random Arrays**  
  Slower than Heap Sort but faster than Insertion Sort for larger datasets.  

- **Sorted Arrays**  
  Comparable to Heap Sort, with slight improvements in recognizing order.  

- **Reverse-Sorted Arrays**  
  Matches Heap Sort performance and outperforms Insertion Sort.  

---

## Limitations  

- **Execution Time**  
  Marginal improvements compared to standard algorithms.  

- **Switching Overhead**  
  Additional computational cost due to method transitions.  

- **Threshold Rigidness**  
  Fixed thresholds may not suit all datasets.  

---

## Future Recommendations  

- Optimize threshold determination to reduce overhead and improve flexibility.  
- Explore other hybrid combinations or enhancements to further boost performance.  
- Investigate domain-specific applications, such as database sorting.

---

## Authors  

- [Cherry Lee Jimenez](https://github.com/cheaneatine)
- [Imroz Mae Khan](https://github.com/imrozkhan214)
- [Junar Landicho](https://github.com/junarlandicho)  

Department of Computer Science  
**University of Science and Technology of Southern Philippines**