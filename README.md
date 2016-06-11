# hello-world
following a tutorial

what could i do here?

public static int Partition(Comparable[] a, int lo, int hi)
{
  int i = lo, j = hi+1;
  Comparable v = a[lo];
  while (true)
  {
    while(Less(a[++i], v))  if (i == hi) break;
    while(Less(v, a[--j]))  if (j == lo) break;
    if (i >= j) break;
    Exch(i,j);
  }
  Exch(v,j);
  return j;
}
