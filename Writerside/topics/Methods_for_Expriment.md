# Methods for Organizing Your Code and Results.

## Coding

### I) How to Read Others Code?
When you download a copy of the code project, you should read the **README** file first, in this file, you will get some useful information: 
- How to run this code? (We can know the entry of this program.)
- Where is the data we need?

Okay, assuming you have read the **README** file,  

xxx

If you have any questions about this code you downloaded, you can check the Github issues page. Maybe someone else has had the same question as you and got the answer there.

### II) Some Tips for Coding Process.
* Don't put all functions in main.py, please classify them according to their functions.
* Jupyter Notebook is a good helper for beginner, easy to use and record the result. However, in the long run, it's more reasonable to encapsulate our code and make it with high modularity(Easy to reuse).
* For those who focus on the transformer-based research job. **Fixing Random Seed** is a good habit. In the **transformers** library, there is a `set_seed` function we can use:
```python
from transformers import set_seed
set_seed(2024)
````

## Results

wandb

log library