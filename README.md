# Kumulatif-Toplam

# Koşan Toplam (Running Sum) Algoritması

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

### Örnek 2:
**Girdi:**  
`nums = [1,1,1,1,1]`  
**Çıktı:**  
`[1,2,3,4,5]`  
**Açıklama:**  
Koşan toplam şu şekilde elde edilir: `[1, 1+1, 1+1+1, 1+1+1+1, 1+1+1+1+1]`.

### Örnek 3:
**Girdi:**  
`nums = [3,1,2,10,1]`  
**Çıktı:**  
`[3,4,6,16,17]`

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
