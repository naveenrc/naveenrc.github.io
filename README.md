## Latest posts

## <a name='downloaddynamic'>Download data from dynamic websites</a>
Lets say we need to download data from a website which is dynamic.<br>
If we do
```bash
wget 'url'
```
Output is a script which you got nothing to do with like this
![image](https://user-images.githubusercontent.com/30205620/29646283-8a02a390-8850-11e7-8152-317991d6e8b2.png)

Url used in the image: https://s3.amazonaws.com/tripdata/index.html

## How to deal with this
We can use
+ python
+ selenium
+ wget
+ BeautifulSoup
+ phantom js (download and save the executable in a folder, we will use it later)

```python
import wget

# html parser
from bs4 import BeautifulSoup

from selenium import webdriver
# webdriver wait is similar to sleep
from selenium.webdriver.support.ui import WebDriverWait
# expected conditions is used to wait until an element in the page is rendered
from selenium.webdriver.support import expected_conditions as EC
# By is used to select an element by a path, say XPATH
from selenium.webdriver.common.by import By

# phantomjs is used to avoid selenium perform operations in a browser
driver = webdriver.PhantomJS(executable_path='path to executable phantomjs along with phantomjs.exe')
        
driver.get("https://s3.amazonaws.com/tripdata/index.html")

# wait for 10 seconds and then until <a></a> elements are rendered
WebDriverWait(driver, 10).until(EC.visibility_of_element_located(
          (By.XPATH, '//*[@id="tbody-content"]/tr[1]/td[1]/a'))
        ) # waits till the element with the specific id appears

src = driver.page_source # gets the html source of the page

parser = BeautifulSoup(src,"lxml") 
# Get the 'a' tag from the source
tag = parser.findAll('a')

for idx,i in enumerate(tag):
    url = i['href'] # get the href attribute of the <a>
	  wget.download(url,out="output path")
```


All your files are downloaded!!!


## <a name='multiprocessing'>Multiprocessing in python</a>
Multiprocessing seems to be a bit difficult but not after reading this
```python
from multiprocessing import Pool, Lock

def func(x, y):
    # do some operations
    with lock:
    # this is like thread safe operation, only one process can access it at a time
    # write ouput to a file or share state using Value or Array from multiprocessing

# making the lock global
def init_child(lock_):
    global lock
    lock = lock_

lock = Lock()
p = Pool('number of processes, example 4', initializer=init_child, initargs=(lock,))
inputs = [1, 2, 3, 4]
p.map(func, inputs)
p.close()
p.join()

```
For more information about multiprocessing, refer https://docs.python.org/2/library/multiprocessing.html

### Contact

LinkedIn: <a href="https://www.linkedin.com/in/naveen-c-823226141/" target="_blank">Naveen Ch </a><br>
Email: naveenrch@yahoo.com<br>
Phone: 832 805 4915
