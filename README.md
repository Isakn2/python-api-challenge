# python-api-challenge
Module 6 challenge
VacationPy and WeatherPy are our coding files.

Output Data
    Pictures for results (8)
    API's retrieved data:
        cities.csv
        hotels.csv

On 'VacationPy.ipynb' code, ThreadPoolExecutor was used because on the previous example, more than 2 hours were needed for the API requests.
ThreadPoolExecutor is part of the concurrent.futures module in Python, which provides a high-level interface for asynchronously executing functions using threads or processes. It's useful when you need to run multiple functions concurrently.

- Definition: max_workers specifies the maximum number of threads that can be used to execute tasks concurrently.
    Default Value: If you don't specify max_workers, the default value is typically the number of processors on your machine multiplied by 5. 
    Impact: Setting a higher number allows more tasks to run simultaneously but can increase memory usage and context switching overhead. A lower number may limit parallelism but could reduce overhead.

The .result() method of a Future object in Python's concurrent.futures module is used to retrieve the result of an asynchronous computation once it has completed.

This approach is ideal for scenarios where tasks involve waiting (like network requests) and can be performed in parallel to improve efficiency and reduce overall execution time.

