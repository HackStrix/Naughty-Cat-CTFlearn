# Naughty Cat 
## CTFlearn
Naughty Cat Writeup

* **Category:** Forensics
* **Points:** 50
* **level:** Medium

## [Challenge](https://ctflearn.com/challenge/890)

> Think the flag is somewhere in there. Would you help me find it?\
> https://ctflearn.com/challenge/download/890

## Solution

The solution is fairly lenghty.
First we use **binwalk** to detect the hidden files 

```
binwalk cut3_c4t.png
```

we get some file here, now lets extract those files

```
binwalk --dd='.*' cut3_c4t.png
```

we get 3 files here, lets detect these file types using **file**

```
file *
```


