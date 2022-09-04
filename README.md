# gnosort: the sorting-agnostic sorting algorithm

```text
 .---. .-. .-. .----.  .----. .----. .----.  .---. 
/   __}|  `| |/  {}  \{ {__  /  {}  \| {}  }{_   _}
\  {_ }| |\  |\      /.-._} }\      /| .-. \  | |  
 `---' `-' `-' `----' `----'  `----' `-' `-'  `-'  
```

O(1) sorting which leverages relativism to produce instantaneous results. 
  
[It started with a tweet](https://twitter.com/ctrlcreep/status/1566073798188826624). Now, it's reality. (Actually, it was [two tweets](https://twitter.com/ctrlcreep/status/1565859604206157824), but who's counting? Not us, because quantity is relative.)

This module exports two functions: 

## 1. gnosort (`gno`)

Sorts an array. Since no one can really say whether one number is larger or 
smaller than another, we can easily achieve O(1) efficiency by simply 
returning the original array. Order is an illusion anyway.
 
```js
const gno = function(arr) {
  return arr
}
```

## 2. aaannb sort (`aaanb`)

Sorts an array by returning an image of a banana. Violates a number of sorting algorithm invariants, but invariancy is just one of those things that's up to the individual to define.

```js
const aaabnn = (arr) => `data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADwAAAAtCAYAAADydghMAAAE/0lEQVRoQ9VaLVcbQRQdzkEgIhCICAQiAoFAICoR/QmICgSiAoGojIxEViAQFRUIREVlBaISgaioqIhAVEQgIiIQOaedu+SmN2/fzC4hJZs5J2c/Znbn3Xn3fc1mbT2EP6HhLcoYxvGHoza9vxE7HuMPRzuW4/Ds2ioAhqAKNrUAAKvgeM7FaK0iYIDAD9q0CwFgXgPQUfytJGCP0gBS1ThmhtK4iZWDDTStkdI8ejZNDbPPsqFkwwB8vB/C5Y+mwf1nw7RHS2dcpyidteH3eyF8vO2GVuu8Maitd6Zg9j4Bq+NSEEkbRgd+g4ZAfi5gKza990E7EZYwwUnU9KefzUCci7+UMEVnUp3vSMbhk93owKIHu75fLuhc0qGS5eyXYJMapkM42lkNwNY7eypyw5I18H7/OLQ7V8tVcZzdy7Ksl36xht9F7V7enoXH0XCpoHNxl31VYEFltLvohZM2fBrjce/LcTGwd3TViNjMRCKXdFDzGEMaAzDAJm14ODgr0XiZmk45LqV1Lo+mhjG+pGGCXW+1wng0CjiyjQa/l0Zva8derOU9m3gc5igNwArSvvi1QaeSjpTTUpun1t9MAJc0DLs9/+YDXt94enwcg/MyQKc2ALTw18XBeGZYkJu0nqF0DnCxogY07s0btlL5rtKS5ymw7PfsV/Nq1MKk9Qzg4w4qpe4U2HRCpFymAfzjw8OzwpYXYjwwpcmcG6nCQRdBMyzenwGMdPLirlv0UZt2LlBa+0jx/ZigeMWGeljW2bnYStvUmpza4p5VYVoTyg7Gvez6fDjohUEUDGEJbQYwXnwfs6tWe7s2YJ0N4NE2Y2mp4FT4nBNS7dhNCDz3UAEuh/x0rxdufjlhaVABuA7dCJxjt2QBSqYx0ZbuaGDZRi8A58kImbajHKU4vAjAqUWx5lBn8RY1JgkYEyAWb2xtLWquRrwHtnwdt67cXBr0Go7K3roRks8hxPC+H3YnVV+yeEC19Lmf94BzzP3qjyB0brcvpk40++UB9ry5E4PzijbYLSIGG5hb+akFgxbtMV9j/SxYzFkLMIUbrYhNAyiqvM1IYw11wIE8o1LDqo0me28v6SFIPT4LMGnRJIpToyf7F+Gr5LbULqt5VlXPBkyN/88EpY6N58pUbgUxB9fKaW7AywBOkNsxpnof/BSolp88X+jn0uLTzIIdG+2ye3geqzhf7wADDbJ6sqMULPperGHaNY666qR80T/ZOMhRlbaIzcJO1CCKdk94zlf1aYV1NgoR2jHemQVsS7k6xbq3kzHP92YvpNSxbd3ywXitoadxWIt0fSlpon8WUY1Sq97GWR3hdExKBo7RTQDKwGdsva1yY6wuQknDNPwccA9MHe3bxfIA6z0KqtrGPASotIZSLCt4DSpzcdbiQ9O/LVk6Kni7PUPh7Z9LrBl4FPe0RsfjgbNK4OKqTASsNot+XgN0kWkRMF9qAej/JfS8irIe8KpnuIje9k6de+qolPY0PfTPAK6iZc4zWmGrxtYBzzHYSL/1dgiFqh4D8Tz9DxVZAFanYzVjvR6F8KiqLMkB1mcVDO/jHnYZAQLn+Npz06+/ROpk8U4FPaNh75V1NeU5O9UQhP4uQluN4Ppt5wlYzu5tnzow3T2n4uyO+lqUo3Ba1KR1KLzWeGY9qV0oG/soFAChxeqtoCiucc49Y2tS1DDGkgkaiqxX5jwEaTFh7r/k0c1Yl+cj4wAAAABJRU5ErkJggg==`
```

![](banana.gif)