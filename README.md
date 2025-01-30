# Kumulatif Toplam (Running Sum) Algoritması

![Uploading Kümülatif Toplam Animasyon  kopyası.gif…]()


## Açıklama
Bu algoritma, bir dizinin koşan toplamını (running sum) hesaplar. Her eleman, kendisinden önceki tüm elemanların toplamı ile güncellenir.

## Örnekler

### Örnek 1:
**Girdi:**  
`nums = [1,2,3,4]`  
**Çıktı:**  
`[1,3,6,10]`  
**Açıklama:**  
Koşan toplam şu şekilde elde edilir: `[1, 1+2, 1+2+3, 1+2+3+4]`.


## Python Çözümü

```python
class Solution(object):
    def runningSum(self, nums):
        total = 0
        result = []

        for num in nums:
            total += num
            result.append(total)
        return result 

``` 

# Running Sum Algorithm

## Description
This algorithm calculates the **running sum** (also known as **cumulative sum**) of an array. Each element is updated with the sum of itself and all previous elements.

## Examples

### Example 1:
**Input:**  
`nums = [1,2,3,4]`  
**Output:**  
`[1,3,6,10]`  
**Explanation:**  
The running sum is obtained as follows:  
`[1, 1+2, 1+2+3, 1+2+3+4]`.



## Python Solution

```python
class Solution(object):
    def runningSum(self, nums):
        total = 0
        result = []

        for num in nums:
            total += num
            result.append(total)
        return result



