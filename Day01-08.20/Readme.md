01 - Swap two numbers without a temp variable

Code
```
let a = 5
let b = 10
a = a+b
b = a-b
a = a-b

console.log('A =',a)
console.log('B =',b)
```
Answer
```
C:Day01-08.20>node Entry.js
A = 10
B = 5
```

02 - Find 3 largest numbers in an array using sorting

Code
```
let numbers = [12, 5, 87, 34, 56, 90, 1, 44];
numbers.sort((a,b)=>b-a);
let top3 = numbers.slice(0,3);
console.log("Three largest numbers: ",top3)
```
Answer
```
C:Day01-08.20>node Entry.js
A = 10
B = 5
Three largest numbers:  [ 90, 87, 56 ]
```

03 - Break a whole no into digitsblike 4562-> 4,5,6,2

Code
```
let num = 4562;
let digits = [];

while (num > 0) {
    let digit = num % 10;        
    digits.unshift(digit); 
    num = Math.floor(num / 10); 
}

```
Answer
```
C:Day01-08.20>node Entry.js
[ 4, 5, 6, 2 ]
```

04 - Scale matrix

Code
```
function scaleMatrix(matrix, scalar) {
    let result = [];

    for (let i = 0; i < matrix.length; i++) {
        result[i] = [];
        for (let j = 0; j < matrix[i].length; j++) {
            result[i][j] = matrix[i][j] * scalar; 
        }
    }

    return result;
}

let A = [
    [1, 2],
    [3, 4]
];
let k = 3;

console.log(scaleMatrix(A, k));
```
Answer
```
C:Day01-08.20>node Entry.js
[ [ 3, 6 ], [ 9, 12 ] ]
```

05 - Multiply two matrises

Code
```
function multiplyMatrices(A, B) {
    let rowsA = A.length,
        colsA = A[0].length,
        rowsB = B.length,
        colsB = B[0].length;

    if (colsA !== rowsB) {
        throw new Error("Matrix multiplication not possible: columns of A must equal rows of B");
    }

    let result = Array.from({ length: rowsA }, () => Array(colsB).fill(0));

    for (let i = 0; i < rowsA; i++) {
        for (let j = 0; j < colsB; j++) {
            for (let k = 0; k < colsA; k++) {
                result[i][j] += A[i][k] * B[k][j];
            }
        }
    }
    return result;
}

let A = [
    [1, 2, 3],
    [4, 5, 6]
];
let B = [
    [7, 8],
    [9, 10],
    [11, 12]
];

console.log(multiplyMatrices(A, B));

```
Answer
```
C:Day01-08.20>node Entry.js
[ [ 58, 64 ], [ 139, 154 ] ]
```

06 - 

Code
```

```
Answer
```

```
