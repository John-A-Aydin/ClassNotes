
|      | 7   |                     |     |     |     |     | 6   | 8   | 9   |
| ---- | --- | ------------------- | --- | --- | --- | --- | --- | --- | --- |
|      |     | 18                  |     |     |     |     | 7   |     |     |
|      |     |                     |     |     | 12  |     |     | {8} |     |
| $_6$ |     |                     | 9   |     |     |     | {6} | 31  | {9} |
|      |     |                     |     |     |     |     |     | {8} |     |
|      |     | 5$\binom{2,3}{4,1}$ |     | 22  |     | 22  |     |     |     |
|      |     |                     |     |     |     |     |     |     |     |
|      |     | 9                   |     |     |     |     | 19  |     |     |
|      |     |                     | {8} |     | 14  |     |     | {8} |     |
| 7    |     | {7}                 | 22  | {7} |     |     | {7} | 15  |     |
for i in range(10):
    for j in range(10):
        for k in range(10):
            if (i + j + k == 22):
                print(i,j,k)