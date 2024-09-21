from multiprocessing import Pool
import math
import time

start_time1 = time.time()
def factorial(n):
    return math.factorial(n)

numbers = [x for x in range(1 , 5200 , 2)]

with Pool(processes=4) as pool:
    pool.map(factorial , numbers)
    

end_time1 = time.time()    
print(f"\ntotal processing time with multiprocessing: {end_time1 - start_time1 :.2f}s") # took approximately 3.8 seconds on my machine

start_time2 = time.time()
for i in numbers:
    factorial(i)
end_time2 = time.time()

print(f"\nTotal processing time without  multiprocessing: {end_time2 - start_time2:.2f}s") # took 10.2 seconds on my machine
