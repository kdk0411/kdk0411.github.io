```python
import pandas as pd
```


```python
file_url = 'https://media.githubusercontent.com/media/musthave-ML10/data_source/main/sample.csv'
sample = pd.read_csv(file_url)
```


```python
sample
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
      <th>Var_1</th>
      <th>Var_2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>2</td>
    </tr>
    <tr>
      <th>1</th>
      <td>3</td>
      <td>4</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>5</td>
    </tr>
    <tr>
      <th>3</th>
      <td>5</td>
      <td>6</td>
    </tr>
    <tr>
      <th>4</th>
      <td>3</td>
      <td>2</td>
    </tr>
    <tr>
      <th>5</th>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <th>6</th>
      <td>2</td>
      <td>6</td>
    </tr>
    <tr>
      <th>7</th>
      <td>5</td>
      <td>7</td>
    </tr>
    <tr>
      <th>8</th>
      <td>6</td>
      <td>8</td>
    </tr>
    <tr>
      <th>9</th>
      <td>7</td>
      <td>4</td>
    </tr>
    <tr>
      <th>10</th>
      <td>7</td>
      <td>7</td>
    </tr>
    <tr>
      <th>11</th>
      <td>8</td>
      <td>3</td>
    </tr>
    <tr>
      <th>12</th>
      <td>9</td>
      <td>7</td>
    </tr>
    <tr>
      <th>13</th>
      <td>3</td>
      <td>9</td>
    </tr>
    <tr>
      <th>14</th>
      <td>2</td>
      <td>2</td>
    </tr>
    <tr>
      <th>15</th>
      <td>1</td>
      <td>3</td>
    </tr>
    <tr>
      <th>16</th>
      <td>2</td>
      <td>6</td>
    </tr>
    <tr>
      <th>17</th>
      <td>2</td>
      <td>4</td>
    </tr>
    <tr>
      <th>18</th>
      <td>3</td>
      <td>3</td>
    </tr>
  </tbody>
</table>
</div>



## DataFrame의 다양한 함수


```python
sample.head
```




    <bound method NDFrame.head of     Var_1  Var_2
    0       1      2
    1       3      4
    2       2      5
    3       5      6
    4       3      2
    5       1      1
    6       2      6
    7       5      7
    8       6      8
    9       7      4
    10      7      7
    11      8      3
    12      9      7
    13      3      9
    14      2      2
    15      1      3
    16      2      6
    17      2      4
    18      3      3>




```python
sample.head(3)
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
      <th>Var_1</th>
      <th>Var_2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>2</td>
    </tr>
    <tr>
      <th>1</th>
      <td>3</td>
      <td>4</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>5</td>
    </tr>
  </tbody>
</table>
</div>




```python
sample.tail()
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
      <th>Var_1</th>
      <th>Var_2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>14</th>
      <td>2</td>
      <td>2</td>
    </tr>
    <tr>
      <th>15</th>
      <td>1</td>
      <td>3</td>
    </tr>
    <tr>
      <th>16</th>
      <td>2</td>
      <td>6</td>
    </tr>
    <tr>
      <th>17</th>
      <td>2</td>
      <td>4</td>
    </tr>
    <tr>
      <th>18</th>
      <td>3</td>
      <td>3</td>
    </tr>
  </tbody>
</table>
</div>




```python
sample.tail(10)
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
      <th>Var_1</th>
      <th>Var_2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>9</th>
      <td>7</td>
      <td>4</td>
    </tr>
    <tr>
      <th>10</th>
      <td>7</td>
      <td>7</td>
    </tr>
    <tr>
      <th>11</th>
      <td>8</td>
      <td>3</td>
    </tr>
    <tr>
      <th>12</th>
      <td>9</td>
      <td>7</td>
    </tr>
    <tr>
      <th>13</th>
      <td>3</td>
      <td>9</td>
    </tr>
    <tr>
      <th>14</th>
      <td>2</td>
      <td>2</td>
    </tr>
    <tr>
      <th>15</th>
      <td>1</td>
      <td>3</td>
    </tr>
    <tr>
      <th>16</th>
      <td>2</td>
      <td>6</td>
    </tr>
    <tr>
      <th>17</th>
      <td>2</td>
      <td>4</td>
    </tr>
    <tr>
      <th>18</th>
      <td>3</td>
      <td>3</td>
    </tr>
  </tbody>
</table>
</div>




```python
sample.info()
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 19 entries, 0 to 18
    Data columns (total 2 columns):
     #   Column  Non-Null Count  Dtype
    ---  ------  --------------  -----
     0   Var_1   19 non-null     int64
     1   Var_2   19 non-null     int64
    dtypes: int64(2)
    memory usage: 436.0 bytes
    

    Coulumn -> 변수명
    Non-Null Count -> Null이 아닌 데이터 수
    Dtype -> 자료형(데이터 타입)
        Object : 텍스트와 같은 문자(''or"") -> 숫자도 ''or""로 감싸면 Object형임
        int64 : 소수점이 없는 숫자
        float64 : 소수점이 있는 숫자
        bool : True or False
        datetime64 : 날짜/시간 자료형


```python
sample.describe()
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
      <th>Var_1</th>
      <th>Var_2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>19.000000</td>
      <td>19.000000</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>3.789474</td>
      <td>4.684211</td>
    </tr>
    <tr>
      <th>std</th>
      <td>2.529360</td>
      <td>2.310667</td>
    </tr>
    <tr>
      <th>min</th>
      <td>1.000000</td>
      <td>1.000000</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>2.000000</td>
      <td>3.000000</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>3.000000</td>
      <td>4.000000</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>5.500000</td>
      <td>6.500000</td>
    </tr>
    <tr>
      <th>max</th>
      <td>9.000000</td>
      <td>9.000000</td>
    </tr>
  </tbody>
</table>
</div>



## DataFrame 직접 만들기


```python
sample_dic = {'name' : ['John', 'Ann', 'Kevin'], 'age' : [23, 22, 21]}
pd.DataFrame(sample_dic)
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
      <th>name</th>
      <th>age</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>John</td>
      <td>23</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Ann</td>
      <td>22</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Kevin</td>
      <td>21</td>
    </tr>
  </tbody>
</table>
</div>




```python
pd.DataFrame([[1, 2],[3, 4],[5, 6],[7, 8]])
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
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>2</td>
    </tr>
    <tr>
      <th>1</th>
      <td>3</td>
      <td>4</td>
    </tr>
    <tr>
      <th>2</th>
      <td>5</td>
      <td>6</td>
    </tr>
    <tr>
      <th>3</th>
      <td>7</td>
      <td>8</td>
    </tr>
  </tbody>
</table>
</div>




```python
pd.DataFrame([[1, 2],[3, 4],[5, 6],[7, 8]], columns = ['var_1','var_2'], index = ['a','b','c','d'])
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
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>a</th>
      <td>1</td>
      <td>2</td>
    </tr>
    <tr>
      <th>b</th>
      <td>3</td>
      <td>4</td>
    </tr>
    <tr>
      <th>c</th>
      <td>5</td>
      <td>6</td>
    </tr>
    <tr>
      <th>d</th>
      <td>7</td>
      <td>8</td>
    </tr>
  </tbody>
</table>
</div>



## DataFrame_Indexing


```python
file_url = 'https://media.githubusercontent.com/media/musthave-ML10/data_source/main/sample_df.csv'
sample_df = pd.read_csv(file_url, index_col=0)
```


```python
sample_df
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
      <th>a</th>
      <td>2</td>
      <td>2</td>
      <td>1</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <th>b</th>
      <td>4</td>
      <td>3</td>
      <td>3</td>
      <td>7</td>
      <td>1</td>
    </tr>
    <tr>
      <th>c</th>
      <td>5</td>
      <td>4</td>
      <td>6</td>
      <td>3</td>
      <td>5</td>
    </tr>
    <tr>
      <th>d</th>
      <td>1</td>
      <td>4</td>
      <td>5</td>
      <td>6</td>
      <td>7</td>
    </tr>
    <tr>
      <th>e</th>
      <td>4</td>
      <td>5</td>
      <td>7</td>
      <td>8</td>
      <td>3</td>
    </tr>
    <tr>
      <th>f</th>
      <td>5</td>
      <td>4</td>
      <td>8</td>
      <td>9</td>
      <td>4</td>
    </tr>
    <tr>
      <th>g</th>
      <td>7</td>
      <td>5</td>
      <td>2</td>
      <td>0</td>
      <td>6</td>
    </tr>
    <tr>
      <th>h</th>
      <td>8</td>
      <td>8</td>
      <td>1</td>
      <td>7</td>
      <td>8</td>
    </tr>
    <tr>
      <th>i</th>
      <td>2</td>
      <td>3</td>
      <td>5</td>
      <td>2</td>
      <td>1</td>
    </tr>
    <tr>
      <th>j</th>
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
sample_df['var_1']
```




    a    2
    b    4
    c    5
    d    1
    e    4
    f    5
    g    7
    h    8
    i    2
    j    9
    Name: var_1, dtype: int64



## 칼럼 기준으로 인덱싱


```python
sample_df['var_1', 'var_2']
```


    ---------------------------------------------------------------------------

    KeyError                                  Traceback (most recent call last)

    File ~\anaconda3\Lib\site-packages\pandas\core\indexes\base.py:3802, in Index.get_loc(self, key, method, tolerance)
       3801 try:
    -> 3802     return self._engine.get_loc(casted_key)
       3803 except KeyError as err:
    

    File ~\anaconda3\Lib\site-packages\pandas\_libs\index.pyx:138, in pandas._libs.index.IndexEngine.get_loc()
    

    File ~\anaconda3\Lib\site-packages\pandas\_libs\index.pyx:165, in pandas._libs.index.IndexEngine.get_loc()
    

    File pandas\_libs\hashtable_class_helper.pxi:5745, in pandas._libs.hashtable.PyObjectHashTable.get_item()
    

    File pandas\_libs\hashtable_class_helper.pxi:5753, in pandas._libs.hashtable.PyObjectHashTable.get_item()
    

    KeyError: ('var_1', 'var_2')

    
    The above exception was the direct cause of the following exception:
    

    KeyError                                  Traceback (most recent call last)

    Cell In[27], line 1
    ----> 1 sample_df['var_1', 'var_2']
    

    File ~\anaconda3\Lib\site-packages\pandas\core\frame.py:3807, in DataFrame.__getitem__(self, key)
       3805 if self.columns.nlevels > 1:
       3806     return self._getitem_multilevel(key)
    -> 3807 indexer = self.columns.get_loc(key)
       3808 if is_integer(indexer):
       3809     indexer = [indexer]
    

    File ~\anaconda3\Lib\site-packages\pandas\core\indexes\base.py:3804, in Index.get_loc(self, key, method, tolerance)
       3802     return self._engine.get_loc(casted_key)
       3803 except KeyError as err:
    -> 3804     raise KeyError(key) from err
       3805 except TypeError:
       3806     # If we have a listlike key, _check_indexing_error will raise
       3807     #  InvalidIndexError. Otherwise we fall through and re-raise
       3808     #  the TypeError.
       3809     self._check_indexing_error(key)
    

    KeyError: ('var_1', 'var_2')



```python
sample_df[['var_1','var_2']]
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
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>a</th>
      <td>2</td>
      <td>2</td>
    </tr>
    <tr>
      <th>b</th>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <th>c</th>
      <td>5</td>
      <td>4</td>
    </tr>
    <tr>
      <th>d</th>
      <td>1</td>
      <td>4</td>
    </tr>
    <tr>
      <th>e</th>
      <td>4</td>
      <td>5</td>
    </tr>
    <tr>
      <th>f</th>
      <td>5</td>
      <td>4</td>
    </tr>
    <tr>
      <th>g</th>
      <td>7</td>
      <td>5</td>
    </tr>
    <tr>
      <th>h</th>
      <td>8</td>
      <td>8</td>
    </tr>
    <tr>
      <th>i</th>
      <td>2</td>
      <td>3</td>
    </tr>
    <tr>
      <th>j</th>
      <td>9</td>
      <td>3</td>
    </tr>
  </tbody>
</table>
</div>



    이와같이 하나로 합쳐야만 에러가 발생하지 않는다

## 열 기준으로 인덱싱

    .loc[]를 사용하면 열기준으로 인덱싱이 가능하다


```python
sample_df.loc['a']
```




    var_1    2
    var_2    2
    var_3    1
    var_4    4
    var_5    3
    Name: a, dtype: int64




```python
sample_df.loc[['a','b','c']]
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
      <th>a</th>
      <td>2</td>
      <td>2</td>
      <td>1</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <th>b</th>
      <td>4</td>
      <td>3</td>
      <td>3</td>
      <td>7</td>
      <td>1</td>
    </tr>
    <tr>
      <th>c</th>
      <td>5</td>
      <td>4</td>
      <td>6</td>
      <td>3</td>
      <td>5</td>
    </tr>
  </tbody>
</table>
</div>




```python
sample_df.loc['a':'c']
# a~c 까지 인덱싱
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
      <th>a</th>
      <td>2</td>
      <td>2</td>
      <td>1</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <th>b</th>
      <td>4</td>
      <td>3</td>
      <td>3</td>
      <td>7</td>
      <td>1</td>
    </tr>
    <tr>
      <th>c</th>
      <td>5</td>
      <td>4</td>
      <td>6</td>
      <td>3</td>
      <td>5</td>
    </tr>
  </tbody>
</table>
</div>



    iloc를 이용하면 아래와 같이 행위치를 기준으로 인덱싱 가능


```python
sample_df.iloc[[0,1,2]]
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
      <th>a</th>
      <td>2</td>
      <td>2</td>
      <td>1</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <th>b</th>
      <td>4</td>
      <td>3</td>
      <td>3</td>
      <td>7</td>
      <td>1</td>
    </tr>
    <tr>
      <th>c</th>
      <td>5</td>
      <td>4</td>
      <td>6</td>
      <td>3</td>
      <td>5</td>
    </tr>
  </tbody>
</table>
</div>




```python
sample_df.iloc[0:2]
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
      <th>a</th>
      <td>2</td>
      <td>2</td>
      <td>1</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <th>b</th>
      <td>4</td>
      <td>3</td>
      <td>3</td>
      <td>7</td>
      <td>1</td>
    </tr>
  </tbody>
</table>
</div>




```python
sample_df.iloc[0:3]
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
      <th>a</th>
      <td>2</td>
      <td>2</td>
      <td>1</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <th>b</th>
      <td>4</td>
      <td>3</td>
      <td>3</td>
      <td>7</td>
      <td>1</td>
    </tr>
    <tr>
      <th>c</th>
      <td>5</td>
      <td>4</td>
      <td>6</td>
      <td>3</td>
      <td>5</td>
    </tr>
  </tbody>
</table>
</div>




```python
sample_df.iloc[0:3, 2:4]
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
      <th>var_3</th>
      <th>var_4</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>a</th>
      <td>1</td>
      <td>4</td>
    </tr>
    <tr>
      <th>b</th>
      <td>3</td>
      <td>7</td>
    </tr>
    <tr>
      <th>c</th>
      <td>6</td>
      <td>3</td>
    </tr>
  </tbody>
</table>
</div>



    .drop을 이용하여 var_1을 제거하는 방법, axis=1을 지정하면 컬럼에 접근


```python
sample_df.drop('var_1', axis=1)
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
      <th>var_2</th>
      <th>var_3</th>
      <th>var_4</th>
      <th>var_5</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>a</th>
      <td>2</td>
      <td>1</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <th>b</th>
      <td>3</td>
      <td>3</td>
      <td>7</td>
      <td>1</td>
    </tr>
    <tr>
      <th>c</th>
      <td>4</td>
      <td>6</td>
      <td>3</td>
      <td>5</td>
    </tr>
    <tr>
      <th>d</th>
      <td>4</td>
      <td>5</td>
      <td>6</td>
      <td>7</td>
    </tr>
    <tr>
      <th>e</th>
      <td>5</td>
      <td>7</td>
      <td>8</td>
      <td>3</td>
    </tr>
    <tr>
      <th>f</th>
      <td>4</td>
      <td>8</td>
      <td>9</td>
      <td>4</td>
    </tr>
    <tr>
      <th>g</th>
      <td>5</td>
      <td>2</td>
      <td>0</td>
      <td>6</td>
    </tr>
    <tr>
      <th>h</th>
      <td>8</td>
      <td>1</td>
      <td>7</td>
      <td>8</td>
    </tr>
    <tr>
      <th>i</th>
      <td>3</td>
      <td>5</td>
      <td>2</td>
      <td>1</td>
    </tr>
    <tr>
      <th>j</th>
      <td>3</td>
      <td>7</td>
      <td>6</td>
      <td>5</td>
    </tr>
  </tbody>
</table>
</div>




```python
sample_df.drop(['var_1', 'var_2'], axis=1)
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
      <th>var_3</th>
      <th>var_4</th>
      <th>var_5</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>a</th>
      <td>1</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <th>b</th>
      <td>3</td>
      <td>7</td>
      <td>1</td>
    </tr>
    <tr>
      <th>c</th>
      <td>6</td>
      <td>3</td>
      <td>5</td>
    </tr>
    <tr>
      <th>d</th>
      <td>5</td>
      <td>6</td>
      <td>7</td>
    </tr>
    <tr>
      <th>e</th>
      <td>7</td>
      <td>8</td>
      <td>3</td>
    </tr>
    <tr>
      <th>f</th>
      <td>8</td>
      <td>9</td>
      <td>4</td>
    </tr>
    <tr>
      <th>g</th>
      <td>2</td>
      <td>0</td>
      <td>6</td>
    </tr>
    <tr>
      <th>h</th>
      <td>1</td>
      <td>7</td>
      <td>8</td>
    </tr>
    <tr>
      <th>i</th>
      <td>5</td>
      <td>2</td>
      <td>1</td>
    </tr>
    <tr>
      <th>j</th>
      <td>7</td>
      <td>6</td>
      <td>5</td>
    </tr>
  </tbody>
</table>
</div>




```python
sample_df.drop(['a','b','c'])
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
      <th>d</th>
      <td>1</td>
      <td>4</td>
      <td>5</td>
      <td>6</td>
      <td>7</td>
    </tr>
    <tr>
      <th>e</th>
      <td>4</td>
      <td>5</td>
      <td>7</td>
      <td>8</td>
      <td>3</td>
    </tr>
    <tr>
      <th>f</th>
      <td>5</td>
      <td>4</td>
      <td>8</td>
      <td>9</td>
      <td>4</td>
    </tr>
    <tr>
      <th>g</th>
      <td>7</td>
      <td>5</td>
      <td>2</td>
      <td>0</td>
      <td>6</td>
    </tr>
    <tr>
      <th>h</th>
      <td>8</td>
      <td>8</td>
      <td>1</td>
      <td>7</td>
      <td>8</td>
    </tr>
    <tr>
      <th>i</th>
      <td>2</td>
      <td>3</td>
      <td>5</td>
      <td>2</td>
      <td>1</td>
    </tr>
    <tr>
      <th>j</th>
      <td>9</td>
      <td>3</td>
      <td>7</td>
      <td>6</td>
      <td>5</td>
    </tr>
  </tbody>
</table>
</div>



## DataFrame Index 변경


```python
sample_df.reset_index()
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
      <th>index</th>
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
      <td>a</td>
      <td>2</td>
      <td>2</td>
      <td>1</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <th>1</th>
      <td>b</td>
      <td>4</td>
      <td>3</td>
      <td>3</td>
      <td>7</td>
      <td>1</td>
    </tr>
    <tr>
      <th>2</th>
      <td>c</td>
      <td>5</td>
      <td>4</td>
      <td>6</td>
      <td>3</td>
      <td>5</td>
    </tr>
    <tr>
      <th>3</th>
      <td>d</td>
      <td>1</td>
      <td>4</td>
      <td>5</td>
      <td>6</td>
      <td>7</td>
    </tr>
    <tr>
      <th>4</th>
      <td>e</td>
      <td>4</td>
      <td>5</td>
      <td>7</td>
      <td>8</td>
      <td>3</td>
    </tr>
    <tr>
      <th>5</th>
      <td>f</td>
      <td>5</td>
      <td>4</td>
      <td>8</td>
      <td>9</td>
      <td>4</td>
    </tr>
    <tr>
      <th>6</th>
      <td>g</td>
      <td>7</td>
      <td>5</td>
      <td>2</td>
      <td>0</td>
      <td>6</td>
    </tr>
    <tr>
      <th>7</th>
      <td>h</td>
      <td>8</td>
      <td>8</td>
      <td>1</td>
      <td>7</td>
      <td>8</td>
    </tr>
    <tr>
      <th>8</th>
      <td>i</td>
      <td>2</td>
      <td>3</td>
      <td>5</td>
      <td>2</td>
      <td>1</td>
    </tr>
    <tr>
      <th>9</th>
      <td>j</td>
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
sample_df.reset_index(drop=True)
# 이전 추가한 index 없이 출력하는 방법
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
sample_df.set_index('var_1')
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
      <th>var_2</th>
      <th>var_3</th>
      <th>var_4</th>
      <th>var_5</th>
    </tr>
    <tr>
      <th>var_1</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>1</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <th>4</th>
      <td>3</td>
      <td>3</td>
      <td>7</td>
      <td>1</td>
    </tr>
    <tr>
      <th>5</th>
      <td>4</td>
      <td>6</td>
      <td>3</td>
      <td>5</td>
    </tr>
    <tr>
      <th>1</th>
      <td>4</td>
      <td>5</td>
      <td>6</td>
      <td>7</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5</td>
      <td>7</td>
      <td>8</td>
      <td>3</td>
    </tr>
    <tr>
      <th>5</th>
      <td>4</td>
      <td>8</td>
      <td>9</td>
      <td>4</td>
    </tr>
    <tr>
      <th>7</th>
      <td>5</td>
      <td>2</td>
      <td>0</td>
      <td>6</td>
    </tr>
    <tr>
      <th>8</th>
      <td>8</td>
      <td>1</td>
      <td>7</td>
      <td>8</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>5</td>
      <td>2</td>
      <td>1</td>
    </tr>
    <tr>
      <th>9</th>
      <td>3</td>
      <td>7</td>
      <td>6</td>
      <td>5</td>
    </tr>
  </tbody>
</table>
</div>



## DataFrame 변수별 계산

|이름|함수|
|:---:|:---:|
|데이터 개수|count()|
|합|sum()|
|평균|mean()|
|중윗값|median()|
|분산|var()|
|표준편차|std()|


```python
sample_df.sum()
```




    var_1    47
    var_2    41
    var_3    45
    var_4    52
    var_5    43
    dtype: int64




```python
sample_df.aggregate(['sum','mean'])
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
      <th>sum</th>
      <td>47.0</td>
      <td>41.0</td>
      <td>45.0</td>
      <td>52.0</td>
      <td>43.0</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>4.7</td>
      <td>4.1</td>
      <td>4.5</td>
      <td>5.2</td>
      <td>4.3</td>
    </tr>
  </tbody>
</table>
</div>



## 그룹별 계산


```python
file_url = 'https://media.githubusercontent.com/media/musthave-ML10/data_source/main/iris.csv'
iris = pd.read_csv(file_url)
```


```python
iris.head()
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
      <th>sepal length (cm)</th>
      <th>sepal width (cm)</th>
      <th>petal length (cm)</th>
      <th>petal width (cm)</th>
      <th>class</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>6.1</td>
      <td>3.0</td>
      <td>4.6</td>
      <td>1.4</td>
      <td>versicolor</td>
    </tr>
    <tr>
      <th>1</th>
      <td>7.2</td>
      <td>3.0</td>
      <td>5.8</td>
      <td>1.6</td>
      <td>virginica</td>
    </tr>
    <tr>
      <th>2</th>
      <td>6.7</td>
      <td>3.1</td>
      <td>4.4</td>
      <td>1.4</td>
      <td>versicolor</td>
    </tr>
    <tr>
      <th>3</th>
      <td>6.2</td>
      <td>2.9</td>
      <td>4.3</td>
      <td>1.3</td>
      <td>versicolor</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4.6</td>
      <td>3.4</td>
      <td>1.4</td>
      <td>0.3</td>
      <td>setosa</td>
    </tr>
  </tbody>
</table>
</div>




```python
iris.groupby('class').mean()
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
      <th>sepal length (cm)</th>
      <th>sepal width (cm)</th>
      <th>petal length (cm)</th>
      <th>petal width (cm)</th>
    </tr>
    <tr>
      <th>class</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>setosa</th>
      <td>5.006</td>
      <td>3.428</td>
      <td>1.462</td>
      <td>0.246</td>
    </tr>
    <tr>
      <th>versicolor</th>
      <td>5.936</td>
      <td>2.770</td>
      <td>4.260</td>
      <td>1.326</td>
    </tr>
    <tr>
      <th>virginica</th>
      <td>6.588</td>
      <td>2.974</td>
      <td>5.552</td>
      <td>2.026</td>
    </tr>
  </tbody>
</table>
</div>




```python
iris.groupby('class').agg(['count', 'mean'])
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead tr th {
        text-align: left;
    }

    .dataframe thead tr:last-of-type th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr>
      <th></th>
      <th colspan="2" halign="left">sepal length (cm)</th>
      <th colspan="2" halign="left">sepal width (cm)</th>
      <th colspan="2" halign="left">petal length (cm)</th>
      <th colspan="2" halign="left">petal width (cm)</th>
    </tr>
    <tr>
      <th></th>
      <th>count</th>
      <th>mean</th>
      <th>count</th>
      <th>mean</th>
      <th>count</th>
      <th>mean</th>
      <th>count</th>
      <th>mean</th>
    </tr>
    <tr>
      <th>class</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>setosa</th>
      <td>50</td>
      <td>5.006</td>
      <td>50</td>
      <td>3.428</td>
      <td>50</td>
      <td>1.462</td>
      <td>50</td>
      <td>0.246</td>
    </tr>
    <tr>
      <th>versicolor</th>
      <td>50</td>
      <td>5.936</td>
      <td>50</td>
      <td>2.770</td>
      <td>50</td>
      <td>4.260</td>
      <td>50</td>
      <td>1.326</td>
    </tr>
    <tr>
      <th>virginica</th>
      <td>50</td>
      <td>6.588</td>
      <td>50</td>
      <td>2.974</td>
      <td>50</td>
      <td>5.552</td>
      <td>50</td>
      <td>2.026</td>
    </tr>
  </tbody>
</table>
</div>



## 변수 내 고윳값 확인하기


```python
iris['class'].unique()
```




    array(['versicolor', 'virginica', 'setosa'], dtype=object)




```python
iris['class'].nunique()
```




    3




```python
iris['class'].value_counts()
```




    versicolor    50
    virginica     50
    setosa        50
    Name: class, dtype: int64



## DataFrame 합치기


```python
left_url = 'https://media.githubusercontent.com/media/musthave-ML10/data_source/main/left.csv'
right_url = 'https://media.githubusercontent.com/media/musthave-ML10/data_source/main/right.csv'

left = pd.read_csv(left_url)
right = pd.read_csv(right_url)
```


```python
left
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
      <th>key</th>
      <th>var_1</th>
      <th>var_2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>a</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <th>1</th>
      <td>b</td>
      <td>3</td>
      <td>2</td>
    </tr>
    <tr>
      <th>2</th>
      <td>c</td>
      <td>4</td>
      <td>4</td>
    </tr>
    <tr>
      <th>3</th>
      <td>d</td>
      <td>2</td>
      <td>3</td>
    </tr>
    <tr>
      <th>4</th>
      <td>e</td>
      <td>1</td>
      <td>0</td>
    </tr>
  </tbody>
</table>
</div>




```python
right
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
      <th>key</th>
      <th>var_3</th>
      <th>var_4</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>b</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <th>1</th>
      <td>c</td>
      <td>6</td>
      <td>5</td>
    </tr>
    <tr>
      <th>2</th>
      <td>e</td>
      <td>3</td>
      <td>8</td>
    </tr>
    <tr>
      <th>3</th>
      <td>f</td>
      <td>2</td>
      <td>7</td>
    </tr>
    <tr>
      <th>4</th>
      <td>g</td>
      <td>3</td>
      <td>4</td>
    </tr>
  </tbody>
</table>
</div>



    merge() 함수를 사용하면 결합이 가능하다


```python
left.merge(right)
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
      <th>key</th>
      <th>var_1</th>
      <th>var_2</th>
      <th>var_3</th>
      <th>var_4</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>b</td>
      <td>3</td>
      <td>2</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <th>1</th>
      <td>c</td>
      <td>4</td>
      <td>4</td>
      <td>6</td>
      <td>5</td>
    </tr>
    <tr>
      <th>2</th>
      <td>e</td>
      <td>1</td>
      <td>0</td>
      <td>3</td>
      <td>8</td>
    </tr>
  </tbody>
</table>
</div>




```python
left.merge(right, on = {'원하는 변수'})
```

    on을 사용하면 공통으로 존재하는 변수를 찾아 키값으로 활용할 수 있다.


```python
# 전체 조인
left.merge(right, how = 'outer')
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
      <th>key</th>
      <th>var_1</th>
      <th>var_2</th>
      <th>var_3</th>
      <th>var_4</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>a</td>
      <td>1.0</td>
      <td>1.0</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>1</th>
      <td>b</td>
      <td>3.0</td>
      <td>2.0</td>
      <td>4.0</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>c</td>
      <td>4.0</td>
      <td>4.0</td>
      <td>6.0</td>
      <td>5.0</td>
    </tr>
    <tr>
      <th>3</th>
      <td>d</td>
      <td>2.0</td>
      <td>3.0</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>4</th>
      <td>e</td>
      <td>1.0</td>
      <td>0.0</td>
      <td>3.0</td>
      <td>8.0</td>
    </tr>
    <tr>
      <th>5</th>
      <td>f</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2.0</td>
      <td>7.0</td>
    </tr>
    <tr>
      <th>6</th>
      <td>g</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>3.0</td>
      <td>4.0</td>
    </tr>
  </tbody>
</table>
</div>




```python
# 왼쪽 조인
left.merge(right, how='left')
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
      <th>key</th>
      <th>var_1</th>
      <th>var_2</th>
      <th>var_3</th>
      <th>var_4</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>a</td>
      <td>1</td>
      <td>1</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>1</th>
      <td>b</td>
      <td>3</td>
      <td>2</td>
      <td>4.0</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>c</td>
      <td>4</td>
      <td>4</td>
      <td>6.0</td>
      <td>5.0</td>
    </tr>
    <tr>
      <th>3</th>
      <td>d</td>
      <td>2</td>
      <td>3</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>4</th>
      <td>e</td>
      <td>1</td>
      <td>0</td>
      <td>3.0</td>
      <td>8.0</td>
    </tr>
  </tbody>
</table>
</div>




```python
left.join(right)
```


    ---------------------------------------------------------------------------

    ValueError                                Traceback (most recent call last)

    Cell In[70], line 1
    ----> 1 left.join(right)
    

    File ~\anaconda3\Lib\site-packages\pandas\core\frame.py:9979, in DataFrame.join(self, other, on, how, lsuffix, rsuffix, sort, validate)
       9816 def join(
       9817     self,
       9818     other: DataFrame | Series | list[DataFrame | Series],
       (...)
       9824     validate: str | None = None,
       9825 ) -> DataFrame:
       9826     """
       9827     Join columns of another DataFrame.
       9828 
       (...)
       9977     5  K1  A5   B1
       9978     """
    -> 9979     return self._join_compat(
       9980         other,
       9981         on=on,
       9982         how=how,
       9983         lsuffix=lsuffix,
       9984         rsuffix=rsuffix,
       9985         sort=sort,
       9986         validate=validate,
       9987     )
    

    File ~\anaconda3\Lib\site-packages\pandas\core\frame.py:10018, in DataFrame._join_compat(self, other, on, how, lsuffix, rsuffix, sort, validate)
      10008     if how == "cross":
      10009         return merge(
      10010             self,
      10011             other,
       (...)
      10016             validate=validate,
      10017         )
    > 10018     return merge(
      10019         self,
      10020         other,
      10021         left_on=on,
      10022         how=how,
      10023         left_index=on is None,
      10024         right_index=True,
      10025         suffixes=(lsuffix, rsuffix),
      10026         sort=sort,
      10027         validate=validate,
      10028     )
      10029 else:
      10030     if on is not None:
    

    File ~\anaconda3\Lib\site-packages\pandas\core\reshape\merge.py:124, in merge(left, right, how, on, left_on, right_on, left_index, right_index, sort, suffixes, copy, indicator, validate)
         93 @Substitution("\nleft : DataFrame or named Series")
         94 @Appender(_merge_doc, indents=0)
         95 def merge(
       (...)
        108     validate: str | None = None,
        109 ) -> DataFrame:
        110     op = _MergeOperation(
        111         left,
        112         right,
       (...)
        122         validate=validate,
        123     )
    --> 124     return op.get_result(copy=copy)
    

    File ~\anaconda3\Lib\site-packages\pandas\core\reshape\merge.py:775, in _MergeOperation.get_result(self, copy)
        771     self.left, self.right = self._indicator_pre_merge(self.left, self.right)
        773 join_index, left_indexer, right_indexer = self._get_join_info()
    --> 775 result = self._reindex_and_concat(
        776     join_index, left_indexer, right_indexer, copy=copy
        777 )
        778 result = result.__finalize__(self, method=self._merge_type)
        780 if self.indicator:
    

    File ~\anaconda3\Lib\site-packages\pandas\core\reshape\merge.py:729, in _MergeOperation._reindex_and_concat(self, join_index, left_indexer, right_indexer, copy)
        726 left = self.left[:]
        727 right = self.right[:]
    --> 729 llabels, rlabels = _items_overlap_with_suffix(
        730     self.left._info_axis, self.right._info_axis, self.suffixes
        731 )
        733 if left_indexer is not None:
        734     # Pinning the index here (and in the right code just below) is not
        735     #  necessary, but makes the `.take` more performant if we have e.g.
        736     #  a MultiIndex for left.index.
        737     lmgr = left._mgr.reindex_indexer(
        738         join_index,
        739         left_indexer,
       (...)
        744         use_na_proxy=True,
        745     )
    

    File ~\anaconda3\Lib\site-packages\pandas\core\reshape\merge.py:2458, in _items_overlap_with_suffix(left, right, suffixes)
       2455 lsuffix, rsuffix = suffixes
       2457 if not lsuffix and not rsuffix:
    -> 2458     raise ValueError(f"columns overlap but no suffix specified: {to_rename}")
       2460 def renamer(x, suffix):
       2461     """
       2462     Rename the left and right indices.
       2463 
       (...)
       2474     x : renamed column name
       2475     """
    

    ValueError: columns overlap but no suffix specified: Index(['key'], dtype='object')


    key라는 컬럼이 겹치기 때문에 불가능하다


```python
left.drop('key', axis=1).join(right.drop('key', axis=1))
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
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>1</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <th>1</th>
      <td>3</td>
      <td>2</td>
      <td>6</td>
      <td>5</td>
    </tr>
    <tr>
      <th>2</th>
      <td>4</td>
      <td>4</td>
      <td>3</td>
      <td>8</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2</td>
      <td>3</td>
      <td>2</td>
      <td>7</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1</td>
      <td>0</td>
      <td>3</td>
      <td>4</td>
    </tr>
  </tbody>
</table>
</div>




```python
left = left.set_index('key')
right = right.set_index('key')
```


```python
left.join(right)
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
    </tr>
    <tr>
      <th>key</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>a</th>
      <td>1</td>
      <td>1</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>b</th>
      <td>3</td>
      <td>2</td>
      <td>4.0</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>c</th>
      <td>4</td>
      <td>4</td>
      <td>6.0</td>
      <td>5.0</td>
    </tr>
    <tr>
      <th>d</th>
      <td>2</td>
      <td>3</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>e</th>
      <td>1</td>
      <td>0</td>
      <td>3.0</td>
      <td>8.0</td>
    </tr>
  </tbody>
</table>
</div>




```python
# 내부 조인
left.join(right, how='inner')
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
    </tr>
    <tr>
      <th>key</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>b</th>
      <td>3</td>
      <td>2</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <th>c</th>
      <td>4</td>
      <td>4</td>
      <td>6</td>
      <td>5</td>
    </tr>
    <tr>
      <th>e</th>
      <td>1</td>
      <td>0</td>
      <td>3</td>
      <td>8</td>
    </tr>
  </tbody>
</table>
</div>




```python
pd.concat([left,right])
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
    </tr>
    <tr>
      <th>key</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>a</th>
      <td>1.0</td>
      <td>1.0</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>b</th>
      <td>3.0</td>
      <td>2.0</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>c</th>
      <td>4.0</td>
      <td>4.0</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>d</th>
      <td>2.0</td>
      <td>3.0</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>e</th>
      <td>1.0</td>
      <td>0.0</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>b</th>
      <td>NaN</td>
      <td>NaN</td>
      <td>4.0</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>c</th>
      <td>NaN</td>
      <td>NaN</td>
      <td>6.0</td>
      <td>5.0</td>
    </tr>
    <tr>
      <th>e</th>
      <td>NaN</td>
      <td>NaN</td>
      <td>3.0</td>
      <td>8.0</td>
    </tr>
    <tr>
      <th>f</th>
      <td>NaN</td>
      <td>NaN</td>
      <td>2.0</td>
      <td>7.0</td>
    </tr>
    <tr>
      <th>g</th>
      <td>NaN</td>
      <td>NaN</td>
      <td>3.0</td>
      <td>4.0</td>
    </tr>
  </tbody>
</table>
</div>




```python
pd.concat([left, right], axis=1)
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
    </tr>
    <tr>
      <th>key</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>a</th>
      <td>1.0</td>
      <td>1.0</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>b</th>
      <td>3.0</td>
      <td>2.0</td>
      <td>4.0</td>
      <td>3.0</td>
    </tr>
    <tr>
      <th>c</th>
      <td>4.0</td>
      <td>4.0</td>
      <td>6.0</td>
      <td>5.0</td>
    </tr>
    <tr>
      <th>d</th>
      <td>2.0</td>
      <td>3.0</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>e</th>
      <td>1.0</td>
      <td>0.0</td>
      <td>3.0</td>
      <td>8.0</td>
    </tr>
    <tr>
      <th>f</th>
      <td>NaN</td>
      <td>NaN</td>
      <td>2.0</td>
      <td>7.0</td>
    </tr>
    <tr>
      <th>g</th>
      <td>NaN</td>
      <td>NaN</td>
      <td>3.0</td>
      <td>4.0</td>
    </tr>
  </tbody>
</table>
</div>



|함수명|설명|예시|
|:---:|:---:|:---:|
|merge()|특정 컬럼을 기준|left.merge(right, how='left')|
|join()|인덱스를 기준|left.join(right)|
|concat()|행기준(axis=1은 열기준), 내/외부조인만 가능|pd.concat([left, right], axis=1)
