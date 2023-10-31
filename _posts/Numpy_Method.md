```python
import numpy as np
import pandas as pd
```


```python
np.array([1, 2, 3])
```




    array([1, 2, 3])




```python
np.array([[1,2,3],
         [4,5,6],
         [7,8,9]])
```




    array([[1, 2, 3],
           [4, 5, 6],
           [7, 8, 9]])




```python
np.array([1,2,3,4,5])
```




    array([1, 2, 3, 4, 5])




```python
file_url = 'https://media.githubusercontent.com/media/musthave-ML10/data_source/main/sample_df.csv'
sample_df = pd.read_csv(file_url, index_col=0)
```


```python
np.array(sample_df)
```




    array([[2, 2, 1, 4, 3],
           [4, 3, 3, 7, 1],
           [5, 4, 6, 3, 5],
           [1, 4, 5, 6, 7],
           [4, 5, 7, 8, 3],
           [5, 4, 8, 9, 4],
           [7, 5, 2, 0, 6],
           [8, 8, 1, 7, 8],
           [2, 3, 5, 2, 1],
           [9, 3, 7, 6, 5]], dtype=int64)




```python
sample_np = np.array(sample_df)
pd.DataFrame(sample_np)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>0</th>
      <th>1</th>
      <th>2</th>
      <th>3</th>
      <th>4</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2</td>
      <td>2</td>
      <td>1</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <th>1</th>
      <td>4</td>
      <td>3</td>
      <td>3</td>
      <td>7</td>
      <td>1</td>
    </tr>
    <tr>
      <th>2</th>
      <td>5</td>
      <td>4</td>
      <td>6</td>
      <td>3</td>
      <td>5</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1</td>
      <td>4</td>
      <td>5</td>
      <td>6</td>
      <td>7</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>5</td>
      <td>7</td>
      <td>8</td>
      <td>3</td>
    </tr>
    <tr>
      <th>5</th>
      <td>5</td>
      <td>4</td>
      <td>8</td>
      <td>9</td>
      <td>4</td>
    </tr>
    <tr>
      <th>6</th>
      <td>7</td>
      <td>5</td>
      <td>2</td>
      <td>0</td>
      <td>6</td>
    </tr>
    <tr>
      <th>7</th>
      <td>8</td>
      <td>8</td>
      <td>1</td>
      <td>7</td>
      <td>8</td>
    </tr>
    <tr>
      <th>8</th>
      <td>2</td>
      <td>3</td>
      <td>5</td>
      <td>2</td>
      <td>1</td>
    </tr>
    <tr>
      <th>9</th>
      <td>9</td>
      <td>3</td>
      <td>7</td>
      <td>6</td>
      <td>5</td>
    </tr>
  </tbody>
</table>
</div>




```python
sample_df.columns
```




    Index(['var_1', 'var_2', 'var_3', 'var_4', 'var_5'], dtype='object')




```python
pd.DataFrame(sample_np, columns = sample_df.columns)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>var_1</th>
      <th>var_2</th>
      <th>var_3</th>
      <th>var_4</th>
      <th>var_5</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2</td>
      <td>2</td>
      <td>1</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <th>1</th>
      <td>4</td>
      <td>3</td>
      <td>3</td>
      <td>7</td>
      <td>1</td>
    </tr>
    <tr>
      <th>2</th>
      <td>5</td>
      <td>4</td>
      <td>6</td>
      <td>3</td>
      <td>5</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1</td>
      <td>4</td>
      <td>5</td>
      <td>6</td>
      <td>7</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>5</td>
      <td>7</td>
      <td>8</td>
      <td>3</td>
    </tr>
    <tr>
      <th>5</th>
      <td>5</td>
      <td>4</td>
      <td>8</td>
      <td>9</td>
      <td>4</td>
    </tr>
    <tr>
      <th>6</th>
      <td>7</td>
      <td>5</td>
      <td>2</td>
      <td>0</td>
      <td>6</td>
    </tr>
    <tr>
      <th>7</th>
      <td>8</td>
      <td>8</td>
      <td>1</td>
      <td>7</td>
      <td>8</td>
    </tr>
    <tr>
      <th>8</th>
      <td>2</td>
      <td>3</td>
      <td>5</td>
      <td>2</td>
      <td>1</td>
    </tr>
    <tr>
      <th>9</th>
      <td>9</td>
      <td>3</td>
      <td>7</td>
      <td>6</td>
      <td>5</td>
    </tr>
  </tbody>
</table>
</div>




```python
sample_np[0]
```




    array([2, 2, 1, 4, 3], dtype=int64)




```python
sample_np[0,2]
```




    1




```python
sample_np[0:3,2:4]
```




    array([[1, 4],
           [3, 7],
           [6, 3]], dtype=int64)




```python
sample_np[:, 2]
```




    array([1, 3, 6, 5, 7, 8, 2, 1, 5, 7], dtype=int64)




```python
np_a = np.array([[1, 3], [0, -2]])
np_a
```




    array([[ 1,  3],
           [ 0, -2]])




```python
np_a + 10
```




    array([[11, 13],
           [10,  8]])




```python
np_a - 5
```




    array([[-4, -2],
           [-5, -7]])




```python
np_a * 2
```




    array([[ 2,  6],
           [ 0, -4]])




```python
np_a + 10 / 3
```




    array([[4.33333333, 6.33333333],
           [3.33333333, 1.33333333]])




```python
np_b = np.array([[1, 0], [0, 1]])
np_b
```




    array([[1, 0],
           [0, 1]])




```python
np_a + np_b
```




    array([[ 2,  3],
           [ 0, -1]])




```python
np_a - np_b
```




    array([[ 0,  3],
           [ 0, -3]])




```python
np_a * np_b
```




    array([[ 1,  0],
           [ 0, -2]])



    Python에서 행렬 곱을 구하려면 @를 이용해야 한다.


```python
np_a @ np_b
```




    array([[ 1,  3],
           [ 0, -2]])



## 임의의 숫자를 뽑는 random.XXX()함수


```python
np.random.randint(11)
```




    6




```python
np.random.randint(50, 71)
```




    58




```python
np.random.randint(50, 71, 5)
```




    array([58, 56, 52, 50, 64])




```python
np.random.choice(['red', 'green', 'white', 'black', 'blue'], size=3)
```




    array(['blue', 'black', 'white'], dtype='<U5')




```python
np.random.choice(['red', 'green', 'white', 'black', 'blue'], size=3, replace=False)
```




    array(['green', 'black', 'white'], dtype='<U5')



## 일련의 숫자를 만드는 arange() 함수


```python
np.arange(1, 11)
```




    array([ 1,  2,  3,  4,  5,  6,  7,  8,  9, 10])




```python
np.arange(1, 11, 2)
```




    array([1, 3, 5, 7, 9])



## 시작과 끝점을 균등한 간격으로 나누는 linspace() 함수


```python
np.linspace(1, 10, 4)
```




    array([ 1.,  4.,  7., 10.])


