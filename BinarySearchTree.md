# Proje 3

### [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

**Örnek:** root x'dir. root'un sağında y bulunur. Solunda z bulunur vb.

1.  Root 7'dir.
2.  5 < 7 olduğu için 7'nin solunda 5 bulunur.
3.  [ 1 < 7 ] ===> [ 1 < 5 ]
4.  8 > 7 olduğu için 7'nin sağında 8 bulunur. 
5.  [ 3 < 7 ] ===> [ 3 < 5 ] ===> [ 3 > 1 ]
6.  [ 6 < 7 ] ===> [ 6 > 5 ]
7.  [ 0 < 7 ] ===> [ 0 < 5 ] ===> [ 0 < 1 ]
8.  [ 9 > 7 ] ===> [ 9 > 8 ]
9.  [ 4 < 7 ] ===> [ 4 < 5 ] ===> [ 4 > 1 ] ===> [ 4 > 3 ]
10. [ 2 < 7 ] ===> [ 2 < 5 ] ===> [ 2 > 1 ] ===> [ 2 < 3 ]

```
                                                                                7  =>         1.  Root 7'dir.
                                                                               / \      
2.  5 < 7 olduğu için 7'nin solunda 5 bulunur.                                5   8           4.  8 > 7 olduğu için 7'nin sağında 8 bulunur. 
                                                                             / \   \
3.  [ 1 < 7 ] ===> [ 1 < 5 ]  ve  6.  [ 6 < 7 ] ===> [ 6 > 5 ]              1   6   9         8.  [ 9 > 7 ] ===> [ 9 > 8 ]
                                                                           / \         
7.  [ 0 < 7 ] ===> [ 0 < 5 ] ===> [ 0 < 1 ]                                   0   3           5.  [ 3 < 7 ] ===> [ 3 < 5 ] ===> [ 3 > 1 ]
                                                                             / \         
10. [ 2 < 7 ] ===> [ 2 < 5 ] ===> [ 2 > 1 ] ===> [ 2 < 3 ]                  2   4             9.  [ 4 < 7 ] ===> [ 4 < 5 ] ===> [ 4 > 1 ] ===> [ 4 > 3 ]
 
```
