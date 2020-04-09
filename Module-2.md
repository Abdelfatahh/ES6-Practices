# ES6 Practices

## Module 2- Arrow Functios

```javascript 
const race = '100m Dash';
const winners = ['Hunter Gath', 'Singa Song', 'Imda Bos'];

const win = winners.map((winner, i) => {(name: winner, race: race,
place: i }))
```
and if you now ```
console.table(win); ```  it will show you the following table.. 

(index)  | name | race | place
------------- | ------------- | ------------- | -------------
0  | Hunter Gath | 100m Dash | 0
1  | Singa Song | 100m Dash | 1 
2 | Imda Bos | 100m Dash | 2 

the problem in the above table that the place start with 0, so we will make the ``` place: i + 1 ``` 
and the table will be as follows: 

(index)  | name | race | place
------------- | ------------- | ------------- | -------------
0  | Hunter Gath | 100m Dash | 1
1  | Singa Song | 100m Dash | 2 
2 | Imda Bos | 100m Dash | 3

the ``` race: race ``` thing seems a little bit redundant so in ES6 we can use ``` race ``` only. 
so it will look like 

```javascript
const win = winners.map((winner, i) => {(name: winner, race, place: i + 1 })) 
```
