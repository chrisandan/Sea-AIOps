##  Sea-AIOps 
 Sea-AIOps is a project that makes Ops more intelligent, and which is called AI+Ops.Sea-AIOps is based on machine learning and statistics to analyze data.


## Features
So far,it supports outlier-detection and data regression which are the basic of prediction.

* Fast Fourier Transformation outlier detection.
* Outlier detection based on median, also it's a median filter to fill missing value.
* Outlier detection by N sigma.

## How to use
* detecting outliers by fft.
```python
outlier_positions = detect_by_fft(datas, 200)
```

* median filter
```python
    for ii in range(0, len(data), window_size):
        median_filtered_signal += get_median_filtered(np.asanyarray(data[ii: ii + window_size])).tolist()
```

* detecting by N sigma
```python
outlier_positions = detect_by_nsigma(datas, 3)
```


## dependencies
* python3.5
* numpy==1.14.5
* statsmodels==0.9.0
* matplotlib==2.2.2
* pandas==0.23.4
* jsonschema==2.6.0
* influxdb==5.2.0
* urllib3==1.23
* requests==2.20.0

