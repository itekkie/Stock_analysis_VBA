# STOCK-ANALYSIS

## `-Indice-`

- [Overview](#overview-of-project)
- [Results](#results)
  - [Comparing the stock performance](#comparing-the-stock-performance)
  - [Comparing the execution times](#comparing-the-execution-times)
- [Summary](#summary)
  - [The advantages and disadvantages of refactoring code in general](#the-advantages-and-disadvantages-of-refactoring-code-in-general)
  - [The advantages and disadvantages of the original and refactored VBA script](#the-pros-and-cons-of-the-original-and-refactored-VBA-script)

## `Overview of Project`

In the prepared workbook for Steve, he can analyze an entire dataset at the click of a button. Now, he wants to expand the dataset to include the entire stock market over the last few years and he is wondering how much time it takes to calculate data for one year. So, the purpose of the project is to compare 12 stock performances in 2017 and 2018 as well as refactor code to improve runtime of calculation.

## `Results`

### Comparing the stock performance

Based on analysed data to compare the stock performance between 2017 and 2018 there are few things.
Firstly, the 2017 was the most successful year for all markets except TERP which lost about 7% of their cost.

![image](https://user-images.githubusercontent.com/68247343/124628254-47e5f400-de4e-11eb-821c-fc8ecfbd80d3.png)

Also, that is evidence that for DQ the biggest success in 2017 with almost 200% of the growth. However, in the 2018 the price of DQ dropped by -62.6%. The most reliable is ENPH stock which constantly growing besides some collapse for others in 2018.

Additionally, the riskiest with high volunteering is SPWR. They earned less in the successful year and lost more than average in the collapsed year.

Furthermore, in 2017 and 2018 the most failed is TERP and on the contrary the most successful is RUN which returned 84% (the difference in price between the beginning of the year and the end of the year) in the collapsed year. 

### Comparing the execution times

To compare the execution times of the original script and the refactored script that is evidance that by refactoring the code, the script run faster. Let's visualize it. In 2017 the refactored script ran faster than original about in 0.71 sec and 0.76 in 2018.

![2017_runtime](./Resources/VBA_Challenge_2017.png)

![2018_runtime](./Resources/VBA_Challenge_2018.png)

To refactor the original script was changed as:

a) Easy to read
![image](https://user-images.githubusercontent.com/68247343/124638287-c6e02a00-de58-11eb-8b66-6e398dfdf783.png)

b) To avoid copying the same lines 12 times to get the results of 12 stock by creating arrays and loop over it.

![image](https://user-images.githubusercontent.com/68247343/124638446-f68f3200-de58-11eb-9ab9-8c3ba63a4886.png)

c) To run faster by refactoring formats of the outputs.
![image](https://user-images.githubusercontent.com/68247343/124638639-2f2f0b80-de59-11eb-9b08-e9fc89ecc3f8.png)


## `Summary`

### `The advantages and disadvantages of refactoring code in general`

The advantage of refactoring code is it makes the code more efficient by taking less steps, using less memory, improving the logic to make it easier to read, and overall, it is easier to maintain. 
The disadvantages of refactoring code are it can be time consuming, and it can make some errors that influence the run code.

### `The pros and cons of the original and refactored VBA script`

As cons, it can be time consuming of refactoring process.

As pros, it is the execution times of the refactored script run faster than the original script with the same outputs for 2017 and 2018. As well as organised code is easier to maintain and to expand to new functionality.
