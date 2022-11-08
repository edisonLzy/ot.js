源字符串：apple

A编辑的结果：appple -> [retain: 3, insert: 'p', retain: 2]


B编辑的结果：aplle  -> [retain: 2, delete: -1, retain: 1, insert: 'l', retain:1]


A: 3
B: 2

A': [2]
B': [2]

A: 1
B: -1

A': [2]
B': [2, -1]

A: p
B: 1

A': [2, p]
B': [2, -1, 1]

A: 2
B: 1

A': [2, p, 1]
B': [2, -1, 1, 1]

A: 1
B: 'l'

A': [2, p, 1, 1]
B': [2, -1, 1, 1,'l']

A: 1
B: 1

A': [2, p, 1, 1, 1]
B': [2, -1, 1, 1,'l',1]


